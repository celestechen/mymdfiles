```flow
st=>start: 
io=>inputoutput: npcpdr
op_1=>operation: npcpdr is not supposed to be zero
cond_1=>condition: check if npcpdr=0
op_2=>operation: replace npcpdr=1

op_3=>operation: calculate ratio of npcpdr between each pair of two waves
cond_3=>condition: check if any ratio>10
op_4=>operation: pick out and fix outliers manually with last or nearest observation
op_5=>operation: fix npcpoth accordingly

op_6=>operation: calculate ratio=average(npcpdr)/average(SKA) for each case
cond_6=>condition: if ratio>4

op_7=>operation: pick out and calculate diff=avg(npcpdr)-avg(SKA)
sub=>subroutine: Your Subroutine
cond_7=>condition: if abs(diff)>50

op_8=>operation: calculate oth_ratio=npcpoth npcpdr
op_9=>operation: fix npcpdr with SKA values
op_10=>operation: fix npcpoth=npcpdr(fixed) oth_ratio

e=>end: OK


st->op_1->cond_1
cond_1(yes)->op_2->cond_1
cond_1(no)->op_3->cond_3
cond_3(yes)->op_4->op_5->op_3
cond_3(no)->op_6->cond_6
cond_6(yes)->op_7->cond_7
cond_6(no)->e
cond_7(yes)->op_8->op_9->op_10
cond_7(no)->e

```

