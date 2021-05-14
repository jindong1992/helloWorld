# helloWorld

1、生成xmi 使用  ./fsm_gen xxx.xmi生成文件如下：  执行命令 gcc -E include/fsm/StateApp.h -I./include/Common（Fsm_Defn.h先注释35行）

2、将生成的头文件放到include\fsm 文件下；将生成的xxx.c文件放到swc\gen文件下；将test_xx
x.c放到app 目录下

3、在所有的action、guard中加入打印TRACE(PURPLE,"'%s'\n", __func__);

4、执行命令 gcc -E include/fsm/StateApp.h -I./include/Common


将1 复制到xx_status.h中，将2复制到xx_chart.c中实现
(Fsm_Defn.h)需要打开

-3 最外层的状态 FSM_LEVEL_0 FSM_TOP
-2 自己内部装换
-1 没有状态
