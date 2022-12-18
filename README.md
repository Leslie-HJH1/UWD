# 代号:不能说的秘密
- 个人在研
- 类型（暂定）：ACT 开放世界
- 引擎：Unity
- 参考：原神、战双、CoA

## 技术：
### 战斗：
- 动作：
  - 1：Mecanim；***2：Animancer***;***3：Playable***
    - 方案1：非Playable，在角色动画数量大的情况下非常占用CPU，且动画融合方面没有后者自然与方便，参数设置不方便，优点：状态机可视化，学习成本相对低
    - 方案2：Playable，插件，用户任意支配动画数量，根据需求进行定制各自的动画，性能方面得到把控，完善的文档，自然流畅的动画融合，参数设置方便，缺点：状态机非可视化，学习成本相对高，并存在问题不可预知风险
    - 方案3: Playable，官方底层API，稳定，自定义自由度高，学习成本不高不低
  - 案例：
    - 【永劫无间】参考2实现动作动画系统；
    - 官方推荐对于动画数量繁多者使用Playable定制动画系统；
    - 【原神】可能使用1，但肯定经过魔改
- 技能：
  - 1：Flux；***2：Timeline+Playable***；***3：Slate***
  - 案例：
    - 网易、腾讯有使用1；(PS:五哥牛逼！！！)
    - 【原神】&【崩坏3】可能使用2
### AI：
- 怪物&NPC：***1：状态机***；***2：行为树***；3：决策树；***4：GOAP***；5：HTN
  - 案例：
    - 【极度恐慌】使用3；
    - 【地平线零黎明】使用4
- 寻路：1：Unity的Navigation；***2：开源项目RecastNavigation***
  - 案例：
    - 【网易自研引擎】参考2;
    - 【原神】使用2；
    - 【死亡搁浅】参考过2；
    - 【腾讯】工作室魔改2形成自身工具；
### 编辑器：
- 节点：1：NodeGraphProcessor；***2：xNode***；3：Node_Editor_Framework
- 一般：Odin(方便，理由略)
- 时间轴：***1：Slate Cinematic Sequencer***；2：Timeline+Playable
  - 案例：
    - 【天涯明月刀】据调查使用2；
    - 【斗罗大陆·魂师对决】根据分享使用2；
    - 【原神】&【崩坏3】可能使用2
### 相机控制：
- ***Cinemation***(方便，理由略)    
### 渲染：
- 目前直接用的***lilToon***，用于二次元人物渲染
### UI
- 会在UI框架中实现做过的全部系统&活动、基础系统
  
## 美术：
- 由于是学习用，所以用的Unity官方资源或者一些网络资源

## 策划：
- 自己来（还没想好）


## 目前在做：
- 2022.10.7-战斗系统
- 2022.9.4-2022.10.6-基本流程搭建
- 2022.11.1-2022.12.18-同步测试完成(战斗、移动等)



