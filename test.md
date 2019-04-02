


#舆情处理流程图



```flow
flowchat
st=>start: 开始
e=>end: 结束
op1=>operation: 等大家忘了
op2=>operation: 去辟谣
op3=>operation: 找人造一个离谱的谣言
op4=>operation: 放任他们带节奏
op5=>operation: 压制属实情况
op6=>operation: 找人混进去乱带节奏
op7=>operation: 让它发酵一会
op8=>operation: 舆论哗然
op9=>operation: 把这个离谱的谣言辟掉

cond1=>condition: 事件严重?
cond2=>condition: 事件是真的？
cond3=>condition: 有人带节奏？
cond4=>condition: 节奏属实？
cond5=>condition: 没有完成压制？


io1=>inputoutput: 事件出现
io2=>inputoutput: 离谱谣言出现

st->io1->cond1(yes)->cond2(yes)->cond3(yes)->cond4(yes)->op5(right)->cond5(yes)->op6->io2
cond1(no)->op1
cond2(no)->op2
cond3(no)->op3
cond4(no)->op4
cond5(no)->op1
op1->op5
op2(right)->op1
op4->io2
op3->io2
io2->op7
op7->op8
op8->op9
op9->e
op1->e
```




