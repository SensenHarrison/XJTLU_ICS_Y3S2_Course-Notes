- [1. 界面隐喻（Interface metaphors）](#1-界面隐喻interface-metaphors)
  - [1.1 界面隐喻的应用方式](#11-界面隐喻的应用方式)
  - [1.2 界面隐喻的优缺点](#12-界面隐喻的优缺点)
- [2. 交互类型](#2-交互类型)
  - [2.1 Instructing（指令式交互）](#21-instructing指令式交互)
  - [2.2 Conversing（对话式交互）](#22-conversing对话式交互)
  - [2.3 Manipulating（操作式交互）](#23-manipulating操作式交互)
    - [2.3.1 直接操作（Direct Manipulation，简称DM）](#231-直接操作direct-manipulation简称dm)
  - [2.4 Exploring（探索式交互）](#24-exploring探索式交互)
  - [2.5 Responding（响应式交互）](#25-responding响应式交互)
  - [2.6 选择适合的交互类型](#26-选择适合的交互类型)
- [3. 界面（Interface）](#3-界面interface)
  - [3.1 界面类型](#31-界面类型)
    - [3.1.1 Command line interfaces（命令行界面）](#311-command-line-interfaces命令行界面)
      - [3.1.需要考虑的因素](#31需要考虑的因素)
    - [3.1.2 Graphical user interfaces (GUIs)（图形用户界面）](#312-graphical-user-interfaces-guis图形用户界面)
      - [3.1.2.1 窗口设计](#3121-窗口设计)
      - [3.1.2.2 菜单样式（Menu styles）](#3122-菜单样式menu-styles)
        - [3.1.2.2.1 需要考虑的因素](#31221-需要考虑的因素)
      - [3.1.2.3 图标设计](#3123-图标设计)
        - [3.1.2.3.1 图标形式（Icon forms）](#31231-图标形式icon-forms)
        - [3.1.2.3.2 图标风格（Icon styles）](#31232-图标风格icon-styles)
          - [3.1.2.3.3 需要考虑的因素](#31233-需要考虑的因素)
    - [3.1.3 Multimedia（多媒体）](#313-multimedia多媒体)
      - [3.1.3.1 需要考虑的因素](#3131-需要考虑的因素)
    - [3.1.4 Virtual reality（虚拟现实）](#314-virtual-reality虚拟现实)
      - [3.1.4.1 应用](#3141-应用)
      - [3.1.4.2 需要考虑的因素](#3142-需要考虑的因素)
    - [3.1.5 网站设计（Website design）](#315-网站设计website-design)
      - [3.1.5.1 可用性与美观性（Usability versus aesthetics）](#3151-可用性与美观性usability-versus-aesthetics)
      - [3.1.5.2 面包屑导航（Breadcrumbs for navigation）](#3152-面包屑导航breadcrumbs-for-navigation)
      - [3.1.5.3 网络广告问题](#3153-网络广告问题)
      - [3.1.5.4 需要考虑的因素](#3154-需要考虑的因素)
    - [3.1.6 移动界面（Mobile interfaces）](#316-移动界面mobile-interfaces)
      - [3.1.6.1 需要考虑的因素](#3161-需要考虑的因素)
    - [3.1.7 家电（Appliances）](#317-家电appliances)
      - [3.1.7.1 需要考虑的因素](#3171-需要考虑的因素)
    - [3.1.8 语音用户界面（Voice User Interfaces）](#318-语音用户界面voice-user-interfaces)
      - [3.1.8.1 模拟人类对话](#3181-模拟人类对话)
      - [3.1.8.2 结构化VUI对话（Structuring VUI dialogs）](#3182-结构化vui对话structuring-vui-dialogs)
      - [3.1.8.3 语音助手（Voice assistants）](#3183-语音助手voice-assistants)
      - [3.1.8.4 需要考虑的因素](#3184-需要考虑的因素)
    - [3.1.9 基于笔的设备（Pen-based devices）](#319-基于笔的设备pen-based-devices)
    - [3.1.10 触摸屏（Touchscreens）](#3110-触摸屏touchscreens)
      - [3.1.10.1 需要考虑的因素](#31101-需要考虑的因素)
    - [3.1.11 基于手势的系统（Gesture-based systems）](#3111-基于手势的系统gesture-based-systems)
      - [3.1.11.1 需要考虑的因素](#31111-需要考虑的因素)
    - [3.1.12  触觉界面（Haptic Interface）](#3112--触觉界面haptic-interface)
      - [3.1.12.1 实时振动触觉反馈（Realtime vibrotactile feedback）](#31121-实时振动触觉反馈realtime-vibrotactile-feedback)
      - [3.1.12.2 需要考虑的因素](#31122-需要考虑的因素)
    - [3.1.13 多模态界面（Multimodal Interfaces）](#3113-多模态界面multimodal-interfaces)
      - [3.1.13.1 跟踪个人动作（Tracking a person’s movements）](#31131-跟踪个人动作tracking-a-persons-movements)
      - [3.1.13.2 需要考虑的因素](#31132-需要考虑的因素)
    - [3.1.14 可共享界面（Shareable interfaces）](#3114-可共享界面shareable-interfaces)
      - [3.1.14.1 需要考虑的因素](#31141-需要考虑的因素)
    - [3.1.15 有形界面（Tangible Interfaces）](#3115-有形界面tangible-interfaces)
      - [3.1.15.1 需要考虑的因素](#31151-需要考虑的因素)
    - [3.1.16 增强现实（Augmented Reality）](#3116-增强现实augmented-reality)
      - [3.1.16.1 使用前置摄像头的AR（AR that uses forward facing camera）](#31161-使用前置摄像头的arar-that-uses-forward-facing-camera)
      - [3.1.16.2 需要考虑的因素](#31162-需要考虑的因素)
    - [3.1.17 可穿戴设备（Wearables）](#3117-可穿戴设备wearables)
      - [3.1.17.1 需要考虑的因素](#31171-需要考虑的因素)
    - [3.1.18 机器人（Robots）](#3118-机器人robots)
      - [3.1.18.1 需要考虑的因素](#31181-需要考虑的因素)
    - [3.1.19 脑机接口（Brain-computer interfaces）](#3119-脑机接口brain-computer-interfaces)
    - [3.1.20 智能界面（Smart interfaces）](#3120-智能界面smart-interfaces)
  - [3.2 选择哪种界面？](#32-选择哪种界面)

# 1. 界面隐喻（Interface metaphors）
界面是被设计成与某种物理实体相似，但同时又具有自身独特属性的一种设计方式。比如桌面隐喻（desktop metaphor）和网络门户（web portals）。
桌面隐喻：计算机桌面的设计灵感来源于现实世界中的办公桌面。在现实的办公桌面上，人们会放置文件、文件夹、便签等物品，方便进行工作和资料管理。计算机桌面借鉴了这种布局方式，用户可以在桌面上放置快捷方式图标（类似于文件和文件夹），通过双击图标来打开相应的应用程序或文件，就像在现实中从办公桌上的文件夹中取出文件查看一样。不过，计算机桌面又具有自身独特的属性，比如可以通过鼠标进行灵活的操作，还能实现文件的快速复制、移动等操作，这些是现实中的办公桌面所不具备的。
网络门户：它就像是一个通往互联网世界的“大门”。在现实生活中，人们通过各种实体的门户进入不同的场所，获取不同的资源和服务。网络门户也类似，用户通过它进入互联网，获取新闻、娱乐、购物等各种信息和服务。例如一些大型的综合门户网站，它会将各种不同类型的信息和功能模块（如新闻板块、视频板块、购物入口等）整合在一起，用户就像在现实世界中通过一个大的门进入一个综合性的场所，然后根据自己的需求选择进入不同的区域获取相应的内容，但网络门户又具有数字化的特点，比如可以根据用户的浏览历史和偏好进行个性化的内容推荐，这是现实中的实体门户所无法做到的。

界面隐喻可以基于活动、物体，或者两者的结合来构建。
基于活动的隐喻：比如电子表格软件中的“工作表”概念。在现实世界中，人们在进行财务核算、数据统计等活动时，会使用纸质的工作表，按照一定的格式填写数据，进行计算和分析。电子表格软件就借鉴了这种活动，用户可以在电子工作表中输入数据、设置公式进行计算等，就像在现实中填写和处理纸质工作表一样。这种基于活动的隐喻，让用户能够凭借对现实活动中使用工作表的经验，快速理解和掌握电子表格软件的基本操作。
基于物体的隐喻：例如手机中的“垃圾桶”图标。在现实生活中，人们将不需要的物品扔进垃圾桶丢弃。手机中的垃圾桶图标也具有类似的功能，用户将不需要的文件、照片等拖入垃圾桶图标，就可以将其删除。这种基于物体的隐喻，直接利用了用户对现实物体（垃圾桶）的认知和使用经验，使用户很容易理解手机中垃圾桶图标的用途。
基于活动和物体结合的隐喻：以在线图书馆为例。它既借鉴了现实生活中人们去图书馆借阅书籍的活动，用户可以在在线图书馆中搜索、借阅、归还电子书籍；同时也借鉴了图书馆这个物体场所的布局和功能，比如有分类的书架（虽然在电脑屏幕上是以虚拟的分类目录形式呈现），用户可以像在现实图书馆中一样，按照分类查找自己需要的书籍。这种结合了活动和物体的隐喻，更全面地利用了用户的现实经验来帮助他们理解和使用在线图书馆。

界面隐喻的作用是利用用户熟悉的认知去帮助用户理解不熟悉的功能。

## 1.1 界面隐喻的应用方式
1. 概念化用户正在做的事情：
通过界面隐喻，让用户能够以一种熟悉的概念来理解他们正在执行的操作。
例如“冲浪互联网”（surfing the Web）。
2. 在界面上实例化的概念模型：
界面隐喻可以将一个抽象的概念模型通过具体的界面元素呈现出来，让用户能够更直观地理解和操作。
例如桌面隐喻（desktop metaphor）和卡片隐喻（card metaphor）。
3. 可视化一个操作：
通过界面隐喻，将一个抽象的操作通过直观的视觉元素呈现出来，让用户能够更直观地理解和执行操作。
例如购物车图标（shopping cart icon）。

## 1.2 界面隐喻的优缺点
优点：
1. Makes learning new systems easier（使学习新系统更容易）
界面隐喻通过利用用户对现实世界中熟悉的事物或活动的认知，降低了用户学习新系统或应用程序的难度。
例如：桌面隐喻和购物车隐喻。
2. Helps users understand the underlying conceptual model（帮助用户理解底层的概念模型）
界面隐喻通过将复杂的系统功能和概念模型以用户熟悉的形式呈现出来，帮助用户更好地理解系统的内部逻辑和工作机制。
例如：文件夹隐喻和时间轴隐喻。
3. Can be very innovative and enable the realm of computers and their applications to be made more accessible to a greater diversity of users（可以非常创新，并使计算机及其应用对更多样化的用户群体更加易于接触）
界面隐喻不仅能够提高用户体验，还可以通过创新的设计方式，使计算机系统和应用程序对更广泛的用户群体更加友好和易于使用。
例如：语音助手和手势控制。

缺点：
1. Break conventional and cultural rules（打破传统和文化规则）
界面隐喻可能会违反用户在现实世界中的传统习惯和文化规则。
例如：回收站放在桌面上和一些文化差异。
2. Can constrain designers in the way that they conceptualize a problem space（限制设计师对问题空间的概念化方式）
界面隐喻可能会限制设计师在思考和解决问题时的创新性和灵活性。
3. Conflicts with design principles（与设计原则冲突）
界面隐喻可能会与一些基本的设计原则相冲突。
简洁性原则：某些隐喻可能会使界面变得过于复杂，增加了用户的认知负担。例如，一个过于复杂的文件夹结构隐喻可能会让用户难以快速找到所需文件，这与简洁性原则相违背。
一致性原则：如果隐喻在不同的上下文中被不一致地使用，可能会让用户感到困惑。例如，如果在某些应用程序中“垃圾桶”图标用于删除文件，而在另一些应用程序中“垃圾桶”图标用于回收文件，这种不一致性会破坏用户对界面的一致性预期。
4. Forces users to understand only the system in terms of the metaphor（迫使用户仅通过隐喻来理解系统）
界面隐喻可能会限制用户对系统的全面理解，使他们只能从隐喻的角度来理解系统功能。
5. Designers can inadvertently use bad existing designs and transfer the bad parts over（设计师可能会无意中使用不良的现有设计，并将不良部分转移过来）
在使用隐喻时，设计师可能会不自觉地借鉴了现有的不良设计，将其中的问题带入新的设计中。
如果现有的某个应用程序中的隐喻设计存在用户体验问题，比如操作不直观或容易出错，而设计师在设计新的应用程序时借鉴了这个隐喻，那么这些问题可能会被延续下来。例如，某个文件管理应用程序中的文件夹隐喻设计不合理，导致用户难以找到文件，如果另一个应用程序也采用了类似的文件夹隐喻，那么用户在使用新应用程序时也会遇到类似的问题。
6. Limits designers’ imagination in coming up with new conceptual models（限制设计师在构思新的概念模型时的想象力）
界面隐喻可能会限制设计师的想象力，使他们难以提出全新的概念模型。
例如，如果设计师总是使用桌面隐喻来设计用户界面，他们可能会难以想象出一种完全不同的、不依赖于桌面概念的文件管理系统。这种依赖隐喻的设计方式可能会阻碍设计师的创新思维，限制他们提出更高效、更符合用户需求的新概念模型。

# 2. 交互类型
交互类型是指用户与系统（如计算机、应用程序、设备等）之间交互的不同方式。这些交互方式可以根据用户的行为和目标进行分类。
以下是五种常见的交互类型：
1. Instructing（指令式交互）。
2. Conversing（对话式交互）。
3. Manipulating（操作式交互）。
4. Exploring（探索式交互）。
5. Responding（响应式交互）。

而交互的范围也包含学习、工作、社交、游戏、浏览、写作、解决问题、决策、搜索、驾驶、导航等。

## 2.1 Instructing（指令式交互）
用户通过明确的指令告诉系统要执行什么操作。
举例：
查看时间：用户可以通过点击时钟图标或输入命令来查看当前时间。
打印文件：用户可以通过选择“打印”选项并指定打印参数来打印文件。
保存文件：用户可以通过选择“保存”选项并指定文件名和保存位置来保存文件。

指令式交互是一种普遍存在的交互方式，适用于多种不同的设备和系统，无论它们的功能和用途如何。
举例：
文字处理软件（Word processors）：用户通过输入命令（如“新建文档”、“保存文档”、“打印文档”等）来操作文档。这些命令通常通过菜单选项或快捷键实现，用户可以快速执行所需的操作。
自动售货机（Vending machines）：用户通过输入选择商品的指令（如按下按钮或输入商品编号）来购买商品。自动售货机会根据用户的指令提供相应的商品。

指令式交互的主要优点是支持快速和高效的交互，而且适用于对多个对象执行重复性操作。
![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/750569b7714f41318792ed3c2c251ce5.png)
![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/4307f99dbf904119b00ca79b90bd2918.png)

## 2.2 Conversing（对话式交互）
用户与系统之间进行类似人类之间对话的交互方式。
其包含从简单的语音识别菜单驱动系统（例如，电话语音应答系统，用户可以说“转接到账户查询”或“查询余额”等）到更复杂的“自然语言”对话（例如，智能助手（如Siri、Google Assistant）可以理解用户的问题并给出相应的回答）。
举例：
时间表：用户可以询问系统关于火车、公交等的时间信息，系统会提供相应的时间表。
搜索引擎：用户可以通过自然语言查询信息，搜索引擎会返回相关的搜索结果。
建议系统：用户可以向系统咨询建议，系统会根据用户的需求提供相应的建议。
帮助系统：用户可以向系统寻求帮助，系统会提供相关的帮助信息和解决方案。
虚拟代理：如虚拟客服代表，可以与用户进行对话，解答用户的问题或处理用户的请求。
聊天机器人：如在线客服聊天机器人，可以与用户进行实时对话，提供信息和服务。
玩具：如语音交互玩具，可以与儿童进行简单的对话和互动。
宠物机器人：如语音交互宠物机器人，可以与用户进行对话和互动，提供陪伴和娱乐。

对话式交互的优点：
1. 让用户（尤其是新手用户）能够以熟悉的方式来与系统交互。
2. 让用户感到舒适、放松，减少恐惧感。

缺点：
1. 当系统无法理解用户所说内容时，可能会产生误解。
2. 语音助手可能会误解儿童的表达。
## 2.3 Manipulating（操作式交互）
用户通过直接操作界面元素或虚拟对象来完成任务。
用户可以通过这些熟悉的动作来操作虚拟对象，如拖动窗口、选择文件、打开文件夹、关闭应用程序和缩放图片等。
用户可以通过物理控制器或空中手势来控制虚拟角色的动作，从而实现更自然的交互方式。
通过在物理对象上添加标记或传感器，用户在物理世界中的操作可以触发相应的数字事件，从而实现物理世界与数字世界的交互。

### 2.3.1 直接操作（Direct Manipulation，简称DM）
直接操作是一种用户交互范式，用户可以直接操作界面中的可视化对象来完成任务。
由本·施耐德曼（Ben Shneiderman）在1983年创造了DM这个术语。
直接操作具有以下三个核心属性：
1. Continuous representation of objects and actions of interest（对感兴趣的对象和动作的持续表示）
含义：在直接操作中，用户感兴趣的对象和动作在界面中持续可见，用户可以直接看到并操作这些对象。
好处：这种持续的表示使用户能够直观地理解对象的状态和位置，以及他们所执行的操作。
2. Rapid reversible actions with immediate feedback on object of interest（对感兴趣的对象进行快速可逆的操作，并提供即时反馈）
含义：在直接操作中，用户可以快速执行可逆的操作，并且系统会立即对用户的操作提供反馈。
好处：
快速性：用户可以迅速执行操作，而不需要等待系统响应。
可逆性：用户可以轻松撤销或修改操作，而不需要担心不可逆的后果。
即时反馈：系统会立即显示用户操作的结果，使用户能够及时了解操作的效果。
3. Physical actions and button pressing instead of issuing commands with complex syntax（使用物理动作和按钮按下，而不是使用复杂的语法发布命令）
含义：在直接操作中，用户通过物理动作（如点击、拖动）或按钮按下来执行操作，而不需要使用复杂的命令语法。
好处：
易用性：用户不需要学习复杂的命令语法，可以直接通过直观的动作来操作界面。
直观性：物理动作和按钮按下更加直观和自然，用户可以更容易地理解和记忆这些操作。

举例： 通过拖放来移动文件。

优点：
1. 新手可以快速学习基本功能。
2. 有经验的用户可以非常快速地执行广泛的任务 - 甚至定义新功能。
3. 间断性用户能够随着时间的推移保持操作概念。
4. 很少需要错误消息。
5. 用户可以立即看到自己的操作是否有助于实现目标，如果没有，可以尝试其他操作。
6. 用户经历较少的焦虑。
7. 用户获得信心和掌握感，感觉在掌控之中。

缺点：
1. 有些人过于字面地理解直接操作的隐喻。例如，有些人可能会期望在iPad上像弹吉他一样操作，但这种直接模拟可能并不适用或有效。
2. 使用鼠标或触摸板移动光标可能比按功能键执行相同操作慢。例如，在执行“查找并替换”这类操作时，使用键盘快捷键可能比用鼠标更快捷。
3. 不支持重复性任务。
4. 某些手势可能比打字更容易出错。例如，尝试通过拖动来将图片的宽度精确调整为2.00厘米可能比直接输入数值更困难且容易出错。

## 2.4 Exploring（探索式交互）
用户通过在虚拟或物理环境中移动来探索和发现信息。
用户可以在计算机生成的虚拟环境中自由移动和探索，如虚拟城市、公园、建筑等。在虚拟环境中，用户可以自由地改变视角和距离，从不同的高度和角度观察环境。
也可以在物理环境中嵌入传感器，当检测到用户的存在时，可以触发数字或物理事件。

## 2.5 Responding（响应式交互）
系统主动向用户发出通知或提醒，提示用户它认为用户可能感兴趣的信息或事件。

系统通过以下方式实现响应式交互：
检测某人的位置和/或在附近的存在，并通过手机或手表通知他们。
根据系统从用户重复行为中学到的信息。

举例：
提醒用户附近有一家咖啡店，一些朋友正在那里聚会
用户的健身追踪器通知他们达到了一个里程碑。

响应式交互的核心特征是系统主动向用户推送通知或提醒，而不需要用户主动请求。

## 2.6 选择适合的交互类型
根据不同的任务或服务我们选择特定的交互类型。
1. 直接操作（Direct manipulation）适合于“执行”类型的任务。
举例：设计（Designing）：用户可以直接拖动和调整设计元素，如在图形设计软件中移动图层或调整颜色。
绘图（Drawing）：用户可以直接在画布上绘制图形，如在绘图软件中使用画笔工具。
飞行（Flying）：用户可以直接控制飞行器的操纵杆或按钮，如在飞行模拟器中控制飞机。
驾驶（Driving）：用户可以直接操作方向盘、油门和刹车，如在赛车游戏中控制赛车。
调整窗口大小（Sizing windows）：用户可以直接拖动窗口的边缘来调整大小，如在操作系统中调整窗口。
2. 发出指令（Issuing instructions）适合于重复性任务。
举例：
拼写检查（Spell checking）：用户可以选择拼写检查功能，让系统自动检查文档中的拼写错误。
文件管理（File management）：用户可以通过命令或菜单选项来复制、移动、删除文件等，如在文件管理器中执行这些操作。
3. 进行对话（Having a conversation）适合于需要获取信息或请求服务的任务。
举例：
查找信息（Finding information）：用户可以通过语音或文本与系统对话，查询天气、新闻、路线等信息，如使用语音助手或聊天机器人。
请求音乐（Requesting music）：用户可以通过语音命令请求播放特定的歌曲或音乐，如使用智能音箱或音乐应用。
4. 混合概念模型（Hybrid conceptual models）适合于支持多种执行相同操作的方式。
举例：
在一些复杂的软件中，用户可以通过直接操作、菜单命令或快捷键等多种方式来完成相同的操作，如在图像编辑软件中，用户可以通过拖动图层、选择菜单选项或使用快捷键来移动图层。

# 3. 界面（Interface）
交互指的是用户与系统进行交流和沟通的过程，包括用户执行的各种操作和系统对这些操作的响应。
举例：
发出指令（Instructing）：用户通过命令或菜单选项告诉系统要执行什么操作，如“保存文件”或“关闭窗口”。
进行对话（Talking）：用户通过语音或文本与系统进行自然语言交流，如询问天气或请求播放音乐。
浏览内容（Browsing）：用户在系统中浏览和查看各种内容，如网页、图片或文档。
做出响应（Responding）：用户对系统提供的信息或提示做出反应，如确认通知或选择推荐的选项。

界面是用户与系统进行交互的媒介和平台，它提供了用户操作和系统响应的机制。
举例：
命令行界面（Command interface）：用户通过输入命令行指令与系统交互，如在终端或命令提示符中输入命令。
菜单驱动界面（Menu-based interface）：用户通过选择菜单选项与系统交互，如在图形用户界面（GUI）中点击菜单按钮。
手势界面（Gesture interface）：用户通过物理手势与系统交互，如在触摸屏设备上滑动或捏合。
语音界面（Voice interface）：用户通过语音命令与系统交互，如使用语音助手或语音识别系统。

## 3.1 界面类型
20种不同类型的界面。
1. Command（命令行界面）：
使用文本命令与计算机进行交互的界面。
2. Graphical（图形用户界面）：
使用图形元素（如窗口、图标、菜单）进行交互的界面。
3. Multimedia（多媒体界面）：
结合文本、图像、音频和视频等多种媒体形式的界面。
4. Virtual reality（虚拟现实界面）：
提供沉浸式3D环境，用户可以通过特殊设备（如VR头盔）进行交互。
5. Web（网页界面）：
通过浏览器访问的基于网络的界面。
6. Mobile（移动界面）：
专为智能手机和平板电脑等移动设备设计的界面。
7. Appliance（设备界面）：
特定设备（如家电、汽车）的专用界面。
8. Voice（语音界面）：
通过语音识别和语音合成进行交互的界面。
9. Pen（笔输入界面）：
使用触控笔在触摸屏或绘图板上进行交互的界面。
10. Touch（触摸界面）：
通过触摸屏幕进行交互的界面。
11. Gesture（手势界面）：
通过识别用户的身体手势（如挥手、指指点点）进行交互的界面。
12. Haptic（触觉界面）：
提供触觉反馈（如振动）以增强交互体验的界面。
13. Multimodal（多模态界面）：
结合多种交互方式（如触摸、语音、手势）的界面。
14. Shareable（共享界面）：
支持多个用户同时访问和交互的界面。
15. Tangible（实体界面）：
通过操作物理对象（如积木、卡片）进行交互的界面。
16. Augmented reality（增强现实界面）：
将数字信息叠加在现实世界中的界面，通常通过AR眼镜或智能手机实现。
17. Wearables（可穿戴界面）：
集成在可穿戴设备（如智能手表、健身追踪器）中的界面。
18. Robots and drones（机器人和无人机界面）：
用于控制和与机器人或无人机进行交互的界面。
19. Brain–computer interaction（脑机交互界面）：
直接通过脑电波与计算机进行交互的界面。
20. Smart（智能界面）：
能够根据用户的行为和偏好进行学习和适应的界面。

### 3.1.1 Command line interfaces（命令行界面）
命令行界面是一种用户通过文本命令与计算机系统进行交互的界面。
用户在命令行提示符下输入特定的命令（这些命令通常是缩写或单词的组合），系统接收到命令后会执行相应的操作并给出反馈。
例如：在Unix或Linux系统中，用户可以输入ls命令来列出当前目录下的所有文件和文件夹。

一些命令是键盘上预设的，而其他命令可以分配给特定的键。
命令行界面的优点在于其搞笑、精确并且快速（Efficient, precise, and fast）。
但是学习一组命令需要较大的学习成本。

#### 3.1.需要考虑的因素
在设计用户界面时，需要研究和确定界面的形式（如何呈现信息）、命名类型（如何命名命令和功能）以及结构（如何组织命令和功能）。
一致性是最重要的设计原则。
这里的命令行界面在网络脚本编写中很受欢迎。
### 3.1.2 Graphical user interfaces (GUIs)（图形用户界面）
图形用户界面是一种用户通过图形元素（如窗口、图标、菜单）与计算机进行交互的界面。
施乐之星（Xerox Star）首次引入了WIMP，催生了GUIs。其中WIMP是窗口（Windows）、图标（Icons）、菜单（Menus）和指针设备（Pointing device，如鼠标）的缩写，是GUI的四个基本组成部分。
1.  Windows（窗口）：窗口是屏幕上可以滚动、拉伸、重叠、打开、关闭和移动的区域。
2. Icons（图标）：图标是代表应用程序、对象、命令和工具的图形符号。
3. Menus（菜单）：菜单是可滚动的选项列表，用户可以从中选择不同的操作。
4. Pointing device（指针设备）：指针设备（如鼠标）用于控制屏幕上的光标，作为用户与窗口、菜单和图标进行交互的入口点。
![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/ca979f6974cb483c9a5298e09c6e4f91.png)
![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/6e7ec5d88ee544439f8f74f870d61ab5.png)
#### 3.1.2.1 窗口设计
窗口的发明是为了克服计算机显示器的物理限制。
窗口允许用户在有限的屏幕空间内查看更多的信息和执行更多的任务，提高了工作效率和灵活性。
窗口内的滚动条可以查看更多信息。
但是多个窗口可能会使找到所需的窗口变得困难。为了解决多个窗口带来的问题，可以采用一些技术来帮助用户更容易地找到和管理窗口。
技术：
列表（Listing）：显示所有打开窗口的列表，用户可以从列表中选择所需的窗口。例如，Windows操作系统中的“任务栏”就提供了这样的功能。
选项卡（Tabbing）：使用选项卡来组织和管理多个窗口或文档，用户可以通过点击不同的选项卡来切换窗口。例如，许多现代浏览器都支持选项卡式浏览。
缩略图（Thumbnails）：显示所有打开窗口的缩略图预览，用户可以通过查看缩略图来快速找到所需的窗口。例如，MacOS中的“Mission Control”功能就提供了这样的预览。

下图是缩略图（Thumbnails）的一个例子。
![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/22b4507a6b834dae90d064378548625c.png)
下图是滚动窗口（A scrolling window）的一个例子。
![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/b3fe9c0bcde9409d86dd02cab8286dc6.png)
#### 3.1.2.2 菜单样式（Menu styles）
有多种菜单样式，下面介绍常见的几种：
1. Flat list（平面列表）
含义：所有菜单选项都在同一层级上以列表形式展示。
优点：适合在显示空间有限的情况下展示大量选项，因为所有选项都在同一平面上，用户可以一目了然地看到所有可用的命令或选项。
2. Drop down（下拉菜单）
含义：菜单选项被组织成层级结构，当用户点击或悬停在某个选项上时，会显示更多的子选项。
优点：可以在相同的屏幕空间内显示更多的选项，特别是当菜单选项具有层级关系时（例如，级联菜单）。
3. Pop-up（弹出菜单）
含义：当用户按下某个命令键或右键点击时，会弹出一个包含相关选项的菜单。
优点：提供了一种快速访问常用命令的方式，特别是与特定项目或任务相关的命令。
4. Contextual（上下文菜单）
含义：根据用户当前的操作或选中的项目，提供与之相关的常用命令。
优点：提高了效率，因为用户可以直接访问与他们当前任务最相关的命令，而不需要在多个菜单中寻找。
5. Collapsible（可折叠菜单）
含义：菜单项可以通过点击标题旁边的+/-图标来展开或折叠其内容。
优点：允许用户根据需要显示或隐藏菜单项，这有助于节省屏幕空间并提高菜单的可管理性。
6. Mega（超级菜单）
含义：所有选项都以二维下拉布局的形式展示，通常包含多个层级和大量的选项。
优点：在一个菜单中展示所有的选项，用户可以通过层级结构快速找到他们需要的命令，而不需要在多个菜单之间切换。

下图展示了Collapsible（可折叠菜单）的例子。
![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/0f394916a332480da898d51658717c2e.png)
下图展示了Mega（超级菜单）的例子。
![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/b3f09e9b7d544c72ac103a926cc1484e.png)

##### 3.1.2.2.1 需要考虑的因素
窗口管理是指用户如何在多个窗口之间进行切换和导航。它使用户能够在不同的窗口（以及监视器）之间流畅地移动。
计应该考虑如何让用户在不同窗口之间切换时保持专注，避免因界面设计不当而分散注意力。
在设计界面时，应遵循一些基本的设计原则，如适当的间距（spacing）、有效的分组（grouping）和保持界面简洁（simplicity），以提高用户体验和界面的可用性。
在设计菜单选项时，需要考虑使用哪些术语来描述操作，这些术语应该直观易懂，以便用户能够快速理解和使用。
一般来说，超级菜单比下拉菜单更容易导航，因为它们以更明显的方式展示所有选项，而下拉菜单可能需要用户多次点击才能找到所需选项。

#### 3.1.2.3 图标设计
图标被认为比命令更容易学习和记忆。
而且图标可以设计得紧凑，并在屏幕上灵活定位。
图标已经成为现代用户界面设计的一个标准组成部分，无论是在桌面应用程序、移动应用还是网页设计中。

自从施乐之星时代以来，图标的外观和感觉已经发生了变化。
早期的图标通常是黑白的，因为当时的显示技术限制了颜色的使用。
而随着技术的进步，图标设计变得更加多样化和丰富。现代图标可以使用颜色、阴影效果、逼真的图像、3D渲染和动画来增强视觉效果和表达力。
为了提高用户体验，许多图标被设计得非常精细和动态。这种设计不仅使图标看起来更加美观，而且能够更有效地传达信息和功能。
通过精心设计，图标可以激发用户的好奇心和兴趣，产生情感共鸣，并给人一种生动和互动的感觉。这种设计有助于提高用户对界面的吸引力和参与度。
![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/fd15e0d9f2874ebb8417b04b38e10814.png)
##### 3.1.2.3.1 图标形式（Icon forms）
图标表示与其所代表对象之间的映射可以是：
1. Similar（相似的）：
图标与其代表的对象在外观上具有相似性。
举例：如一个文件夹图标，通常是一个文件夹的图像，用户可以直接从视觉上识别其代表“文件”这一对象。
2. Analogical（类比的）：
图标通过类比的方式表达其代表的操作或概念。
举例：如剪刀图标通常用来表示“剪切”操作，尽管剪刀本身并不是剪切操作，但通过类比，用户可以理解其代表的含义。
3. Arbitrary（任意的）：
图标与其代表的对象或操作之间没有直观的联系，需要用户通过学习来记忆。
举例：如使用“X”来表示“删除”，这并没有直观的相似性或类比关系，用户需要通过经验或教学来理解其含义。

最有效的图标是相似的图标。
对于动作类的操作，设计直观的图标可能更具挑战性，因为动作不像物体那样容易视觉化。我们可以通过组合物体和符号的方式来设计图标，以便捕捉并表达动作的关键特征。

##### 3.1.2.3.2 图标风格（Icon styles）
有两种风格：
1. User（用户图标）：这些图标通常代表用户界面中与用户相关的功能或操作。
2. Utility（工具图标）：这些图标通常代表应用程序或系统中的工具和实用功能。

![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/6390acbe4b9b468aa1bf80a84e455af3.png)
###### 3.1.2.3.3 需要考虑的因素
设计图标时，有许多可用的资源可以帮助设计师提高效率和质量。
这些资源包括：
Guidelines（指南）：提供设计原则和最佳实践的文档，帮助设计师创建一致且有效的图标。
Style guides（样式指南）：详细说明特定项目或品牌的视觉风格，包括颜色、形状和字体等。
Icon builders（图标构建器）：在线工具或软件，允许设计师快速创建和定制图标。
Libraries（库）：包含大量预设计图标的集合，设计师可以直接使用或作为灵感来源。
Online tutorials（在线教程）：提供图标设计技巧和方法的教学视频或文章。

对于小型图标集，可以结合使用文本标签来帮助识别。
对于大型图标集（例如，照片编辑或文字处理），可以通过悬停（hover）功能来显示每个图标的文本标签或提示信息。

### 3.1.3 Multimedia（多媒体）
多媒体界面将图形、文本、视频、声音和动画等多种媒体形式整合在一起，为用户提供丰富的互动体验。
在多媒体界面中，用户可以通过点击图像或文本中的链接来触发不同的操作或导航到其他内容。
点击链接可能会将用户带到程序的另一部分，如不同的页面、功能或模块。也可能会触发动画或视频片段的播放，为用户提供动态的视觉内容。
多媒体界面通常提供导航选项，允许用户返回之前的位置或继续探索其他内容。
通过结合多种媒体形式，多媒体界面可以更有效地传达复杂或多维的信息。

优点：
1. Facilitates rapid access to multiple representations of information（便于快速访问多种信息表现形式）。
2. Can provide better ways of presenting information than can any media alone（可以提供比任何单一媒体更好的信息呈现方式）。
3. Can enable easier learning, better understanding, more engagement, and more pleasure（可以促进更轻松的学习、更好的理解、更多的参与和更多的乐趣）。
4. Can encourage users to explore different parts of a game or story（可以鼓励用户探索游戏或故事的不同部分）。

缺点：
1. Tendency to play video clips and animations while skimming through accompanying text or diagrams（倾向于在浏览伴随的文本或图表时的视频片段和动画，而忽视文本和图表信息）

#### 3.1.3.1 需要考虑的因素
设计多媒体界面时，需要考虑如何帮助用户有效地处理和整合来自不同媒体的信息。
通过提供互动性强的活动和模拟，用户可以在实践中学习和解决问题。
利用测验、电子笔记本和游戏等工具来增强用户的学习体验。

多媒体特别适合于需要快速浏览和探索大量信息的场景。但是对于长时间阅读不太理想。

### 3.1.4 Virtual reality（虚拟现实）
虚拟现实是通过计算机技术生成的三维图形模拟，为用户提供一种沉浸式的体验。
Gigante在1993年强调虚拟现实的主要特征是让用户感觉自己置身于虚拟环境中，而不是作为一个旁观者从外部观察。
虚拟现实为用户带来了全新的体验方式，允许他们在三维空间中与虚拟物体进行互动和导航。
因为起的沉浸式和互动式的体验，所以它能够极大地吸引和吸引用户。

优点：
1. Can have a higher level of fidelity with objects that they represent compared to multimedia（与多媒体相比，可以对所代表的对象具有更高程度的真实性）。
2. Induces a sense of presence where someone is totally engrossed by the experience（诱导一种存在感，使人完全沉浸在体验中）。
3. Provides different viewpoints: first and third person（提供不同的视角：第一人称和第三人称）。

缺点：
1. Early head-mounted displays were uncomfortable to wear and could cause motion sickness and disorientation（早期的头戴式显示器佩戴不舒适，并可能导致晕动症和迷失方向）
但是随着技术的进步，现代VR头戴式显示器（如HTC Vive）已经变得更加轻便、舒适，并且具有更精确的头部追踪功能。

#### 3.1.4.1 应用
1. Video games（电子游戏）。
2. Arcade games for social groups（面向社交群体的街机游戏）。
3. Therapy for fears（恐惧症治疗）。
4. Experience how others feel emotions（体验他人的情感）。
5. Enrich user’s planning experience for travel destinations（丰富用户对旅游目的地的规划体验）。
6. Architecture, design, and education（建筑、设计和教育）。

下图是一个名为《We wait》的BBC VR短片，讲述了关于叙利亚难民夜间要从土耳其乘走私艇穿过爱琴海偷渡去对岸的希腊的故事。
![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/78b40ff396c64a2a90d8e10c42f6bd59.png)
下图展示了体验博物馆的VR例子。
![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/9482a7c1a4f0489f9b56fe82d3d9b10f.png)
#### 3.1.4.2 需要考虑的因素
研究人员正在探索如何创建既安全又逼真的虚拟现实环境，以提高培训的有效性。
VR也被用于治疗，特别是用于帮助人们面对和克服他们的恐惧。
设计者需要考虑用户如何在虚拟环境中移动和导航，以及是否使用第一人称（用户感觉自己在环境中）或第三人称（用户感觉自己在观察一个角色）视角。
设计者需要确定用户如何与虚拟环境互动，包括如何使用身体动作（如头部和手部运动）来控制虚拟角色或界面元素。
设计者需要考虑用户如何接收和操作信息，包括使用各种输入设备（如键盘、鼠标、操纵杆）来与虚拟环境互动。
为了产生存在感，设计者需要确定虚拟环境的真实性水平，以使用户感到他们真正存在于虚拟环境中。

### 3.1.5 网站设计（Website design）
早期的网站主要是基于文本的，并提供超链接连接不同的页面或网站。
在早期网站设计中，设计师主要关注如何有效地组织和呈现信息，以提高用户的导航效率。
现代网站设计更加注重视觉效果和用户体验，力求使网站在众多网站中脱颖而出。
随着移动设备的普及，网站设计需要适应不同的输入方式和屏幕尺寸。

#### 3.1.5.1 可用性与美观性（Usability versus aesthetics）
简洁、直观、易于使用的设计大多数人都可以接受。
更加复杂、富有创意和视觉冲击力的设计，虽然可能吸引眼球，但可能不易理解和使用。
在设计网站时，需要在用户寻找信息的便利性和网站提供美观愉悦体验之间找到平衡。
用户在网站上的阅读习惯是快速且粗略的。
设计师需要考虑如何通过品牌化设计来吸引用户的注意力，并保持他们的兴趣。

#### 3.1.5.2 面包屑导航（Breadcrumbs for navigation）
面包屑导航是一种显示用户当前位置以及他们如何到达该位置的路径的导航方式，通常以一系列类别标签的形式出现。
它的优点如下：
1. 使用户能够查看其他页面而不会迷失方向。用户可以轻松地跟踪他们的位置，并知道如何返回之前的页面。
2. 非常易用。
3. 提供一键访问更高级别网站层级的能力。
4. 吸引首次访问者在查看登陆页面后继续浏览网站。
 
![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/125c303109de4e2c89127745122845e2.png)
#### 3.1.5.3 网络广告问题
网络广告可能会以打扰用户的方式出现，如弹出窗口、自动播放的视频等，几乎无处不在。
一些网络广告设计得非常醒目（如闪烁的图像或动画），具有攻击性（如强迫用户观看），持续不断（如重复出现的广告），以及令人烦恼（如难以关闭的广告）。
户往往需要采取一些措施（如关闭广告、点击“不再显示”按钮等）才能停止广告的干扰。
可以考虑使用广告拦截器（ad blockers）作为一种应对网络广告侵扰的措施。

#### 3.1.5.4 需要考虑的因素
有许多资源可以帮助设计师学习和应用网站设计的最佳实践和原则。
Veen在2001年提出的设计任何网站时需要考虑的三个核心问题：
1. 我在哪里？
用户需要清楚地知道他们在网站中的位置。
2. 我可以去哪里？
用户需要知道他们可以从当前位置访问哪些其他页面或部分。
3. 这里有什么？
用户需要知道当前页面上有哪些内容和功能。

### 3.1.6 移动界面（Mobile interfaces）
移动界面通常指的是为手持设备设计的界面，这些设备便于携带，可以在移动中使用。
移动设备已经广泛普及，成为人们日常生活和工作中不可或缺的一部分。
例如，手机、健身追踪器和智能手表。
虽然平板电脑的尺寸比手机大，但它们仍然便于携带，适用于移动环境。因此这一部分也包括平板电脑的界面。
例如，空乘人员、销售专业人员、课堂学习。
![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/5bc6d9139f4d44809ac83d1589334272.png)

#### 3.1.6.1 需要考虑的因素
对于手部灵活性差或手指粗大的人来说，移动界面可能难以使用。
关键考虑的是触摸目标区域：
1. 用户在手机显示屏上触摸以触发某个动作的区域，如按键、图标、按钮或应用程序。
2. 空间需要足够大，以便所有手指都能准确按压。
3. 如果太小，用户可能会不小心按错键。
4. 可以使用菲茨定律来帮助设计正确的间距。

所有控件的最小可触摸区域应为44点 x 44点。

### 3.1.7 家电（Appliances）
家电指的是我们日常生活中经常使用的各种设备，这些设备可能位于家中、办公室、公共场所或汽车内。
例如洗衣机、遥控器、烤面包机、打印机和导航系统等。
除了家用电器，个人设备也是我们日常生活中不可或缺的一部分。
例如数字时钟、数码相机等。
用户通常只会在短时间内使用这些设备，完成特定的任务后就会停止使用。
例如启动洗衣机、观看电视节目、购买车票、调整时间或拍摄快照等。
由于用户与这些设备的交互时间较短，因此这些设备的用户界面需要非常直观，用户无需经过复杂的学习过程就能使用。

#### 3.1.7.1 需要考虑的因素
由于用户与这些设备的交互通常是为了完成特定的、短期的任务，因此界面设计应该支持快速、短暂的交互。
界面应该尽可能简洁，避免不必要的复杂性，以便用户可以轻松理解和使用。
设计者需要考虑软控制和硬控制之间的权衡。
硬控制（Hard controls）：如按钮、旋钮、拨盘或物理开关等，它们是物理的、固定的，用户可以直接触摸和操作。
软控制（Soft controls）：如触摸屏上的虚拟按钮、滑动条等，它们是通过软件实现的，可以根据需要动态变化。

### 3.1.8 语音用户界面（Voice User Interfaces）
语音用户界面允许用户通过语音与应用程序进行交互，而不仅仅是通过传统的文本输入或物理按钮。
这种界面可用于查询时间表、规划行程或通过电话服务进行通信。
语音界面特别适合于快速获取特定信息或执行需要快速响应的任务。
用户可以通过语音命令查询航班时间或购买音乐会门票，而无需手动输入信息或浏览网页。
这种界面也适用于视觉障碍人士。
例如，语音识别文字处理器、页面扫描仪、网络阅读器和家庭控制系统。

#### 3.1.8.1 模拟人类对话
在日常对话中，人们常常会在对方讲话时打断对方，尤其是在需要快速决策或表达自己观点的情况下。
例如：在餐厅点餐时，顾客可能会在服务员列举所有选项之前就选择自己想要的菜品，而不是等待服务员念完所有菜单项。
在语音交互系统中，"barge-in"功能允许用户在系统还没有念完所有选项时就选择一个选项。

#### 3.1.8.2 结构化VUI对话（Structuring VUI dialogs）
Directed dialogs are where the system is in control of the conversation（定向对话是指系统控制对话）
在这种类型的对话中，系统引导整个交互过程，包括提出问题和要求特定的回答。
系统提出具体问题并要求特定回答。

在更灵活的系统中，用户可以自由地表达他们的需求，而不需要严格遵循系统的引导。
用户可能会说：“我想下周一去巴黎待两周。”
但这样错误的可能性更大，因为呼叫者可能认为系统像人一样。
当用户偏离了预期的对话流程时，系统可以通过引导提示来帮助用户回到正确的轨道上。
系统可能会说：“对不起，我没有完全理解。您是说您想下周一乘飞机吗？”

#### 3.1.8.3 语音助手（Voice assistants）
语音助手如Alexa、Google Assistant、Siri等，因其便利性和多功能性而在家庭中广泛使用。
语音助手设计为多功能设备，可以满足不同用户的需求，而不仅仅是为某个特定任务设计。
语音助手可以参与家庭活动，提供娱乐和教育内容，增进家庭成员之间的互动。
通过共同参与语音助手支持的活动，家庭成员可以加强彼此之间的联系和理解。
然而，4岁以下的幼儿很难被语音助手理解。当幼儿发现自己无法与语音助手有效沟通时，可能会感到沮丧和挫败，这可能影响他们与技术互动的意愿和体验。

#### 3.1.8.4 需要考虑的因素
设计语音交互系统时，需要确保对话能够顺利进行，即使在用户偏离主题或表达不清晰时也能维持有效的沟通。
语音交互系统应提供清晰的导航提示，使用户能够快速找到他们需要的信息或功能。
系统应允许用户在发生错误时（如误解或操作失误）能够轻松地纠正并继续他们的任务。
系统应能够处理用户的模糊或不明确的请求，并提供适当的指导或澄清问题。

设计语音交互系统时，需要考虑使用哪种类型的声音来与用户交流。
研究用户对不同声音特征的偏好可以帮助设计更符合用户期望的语音交互系统。

### 3.1.9 基于笔的设备（Pen-based devices）
基于笔的设备使用户能够通过笔形输入设备与数字界面进行交互。
由于许多人从小就开始学习绘画和书写，基于笔的设备可以让用户利用这些已有的技能进行数字创作。
数字墨水，例如Anoto，使用普通墨水与数字摄像头的组合，可以数字化记录在特殊纸张上用笔书写的所有内容。
![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/2c5706fc3d5e4cb6bdec7a5b676735ff.png)
优点：
1.  Allows users to annotate existing documents quickly and easily（允许用户快速轻松地注释现有文档）。
2. Can be used to fill in paper-based forms that can readily be converted to a digital record using standard typeface（可用于填写纸质表格，这些表格可以很容易地转换为使用标准字体的数字记录）。
3. Can be used by remote teams to communicate and work on the same documents（可被远程团队用来沟通和协作处理相同的文档）。

### 3.1.10 触摸屏（Touchscreens）
单点触摸屏允许用户通过触摸屏幕来与设备交互，例如选择选项或输入信息。
这种触摸屏常见于需要用户自助服务的场合，如售票机、自动取款机等。

多点触控屏幕可以同时检测多个触摸点，使用户能够进行更复杂的手势操作。
用户可以通过这些手势来执行如滑动浏览、捏合缩放、推动等操作。
多点触控屏幕通过在屏幕上布置的触摸感应网格来检测和识别多个触摸点。
触摸屏技术已经广泛应用于各种便携式和固定式显示设备。
例如智能手机、iPod、平板电脑和桌面电脑。

触摸屏可以识别和响应各种单手和双手手势，提供丰富的交互方式包括敲击、缩放、拉伸、滑动、停留和拖拽。

#### 3.1.10.1 需要考虑的因素
为特定任务提供流畅且直接的交互风格，包括自由手和基于笔的手势。
核心设计关注点包括触摸显示屏的大小、方向和形状是否影响协作。
与使用物理键盘或鼠标相比，直接用手指滑动屏幕来进行滚动和浏览通常更快、更直观。
用户需要学习如何使用多点触控手势。为了降低学习曲线并提高易用性，最好限制常用命令的手势数量。
与物理键盘相比，在触摸屏上使用虚拟键盘进行打字通常更慢、更容易出错，并且使用起来不那么方便。

### 3.1.11 基于手势的系统（Gesture-based systems）
基于手势的系统使用户通过移动他们的手臂和手来与设备或应用程序进行交互。
这些系统通常依赖于摄像头、传感器和计算机视觉算法来检测和解释用户的手势。
基于手势的系统能够在三维空间中识别用户的手势，无论用户在房间的哪个位置。
为了让系统正确理解手势，用户需要按照一定的顺序执行手势，就像句子需要按照语法规则构造一样。
![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/8c854a8680bf4eb796fb64281c4b4f86.png)
#### 3.1.11.1 需要考虑的因素
研究和设计时需要考虑计算机如何检测和识别用户所做的手势。
包括手势的开始和结束点、手势的形状、速度和方向等。
研究和设计时需要区分用户是有意做出的手势（如指向某个对象）还是无意的动作（如挥手）。
在一些应用中，用户的手势可能在界面上有一个图形化的反馈，如虚拟形象或动画。这个图形表现需要足够真实，以便用户能够认同并与之互动，但又不能过于复杂以至于难以实现或影响性能。

### 3.1.12  触觉界面（Haptic Interface）
触觉界面通过对人体施加振动和力量来提供物理反馈。
通过在人身上嵌入的执行器（actuators）如衣物或携带的设备（如智能手机）来施加振动和力量。
智能手机和一些可穿戴设备中内置的振动马达就是触觉反馈的一种常见形式。
振动触觉反馈可以用来模拟想要交流的远程人员之间的触摸感。
超声波触觉技术使用超声波在空中创建可感知的3D形状，从而让用户感觉到仿佛触摸到了实际并不存在的物体。


#### 3.1.12.1 实时振动触觉反馈（Realtime vibrotactile feedback）
这种技术可以在用户演奏小提琴出现错误时提供即时的振动提示。
通过捕捉用户的手臂动作，系统可以检测到与预设模型不一致的动作。
当检测到错误动作时，系统会在用户的手臂或手上产生短促的振动，作为提示。
![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/eb7e2bb2e186451eb42df6689631ebed.png)
还可以使用气泡触觉反馈的人造肌肉外骨骼。
![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/18bf461f599848eca0f46858cf1685a6.png)
#### 3.1.12.2 需要考虑的因素
需要确定在用户身体上的哪些部位放置振动马达（执行器）以提供最有效的触觉反馈。
设计时需要考虑是提供一次性的振动还是一系列连续的振动来传达信息。
需要确定振动发生的时机以及振动的强度。
需要考虑用户在不同环境或情境下对振动触觉反馈的感受。
探索振动触觉反馈在新型应用中的创新用途。
举例：
慢速敲击：模拟水滴的感觉，用来提示即将下雨。
快速敲击：模拟雷暴的临近，用来警告即将到来的雷暴天气。

### 3.1.13 多模态界面（Multimodal Interfaces）
多模态界面通过结合不同的感官模态（如触摸、视觉、听觉和语音）来增强用户的体验。
多模态界面利用多种感官输入和输出方式来传递和接收信息。
多模态界面允许用户以多种方式与计算机进行交互，从而提高交互的灵活性和效率。
在多模态界面中，语音和视觉是最常用的两种模态。
多模态界面可以集成多种传感器来捕捉和分析更多的人体动作和特征。
例如，注视点、面部表情和唇部动作。
多模态界面可以收集用户的多种输入，用于个性化和定制用户界面。

#### 3.1.13.1 跟踪个人动作（Tracking a person’s movements）
Kinect相机可以实时检测多模态输入，使用RGB摄像头进行面部识别和手势识别，深度摄像头进行动作跟踪，以及麦克风进行语音识别。
通过捕捉和分析用户的动作，Kinect可以将用户的动作映射到一个虚拟形象上。

#### 3.1.13.2 需要考虑的因素
多模态交互系统需要能够理解和解释用户的各种行为和输入方式。
多模态系统涉及多种输入和输出方式，这使得系统的校准和优化更加复杂。
研究和设计多模态系统时需要考虑将不同的输入和输出方式结合起来能带来哪些好处。
研究和设计时需要考虑说话和做手势是否是人类与计算机互动的自然方式。

### 3.1.14 可共享界面（Shareable interfaces）
可共享界面是为了支持多个用户同时或依次使用而设计的。
可共享界面通常配备有多个输入设备，有时允许同地用户组同时输入。

人们使用自己的笔或手势的大型墙面显示器或者小组使用指尖与信息互动的交互式桌面。
![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/885b0fc46dd3455f955e1997e956346e.png)

交互式桌面系统的例子如下：
DiamondTouch：由三菱电机（Mitsubishi Electric）开发，支持多点触控和手势识别。
Smart Table：通常指的是智能交互式桌面系统，允许用户通过触摸和手势来操作。
Surface：微软的Surface系列设备，包括平板电脑和交互式桌面，支持多点触控和协作功能。
![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/7bca9fcaf44648df8cb435c3031bd5b1.png)

优点：
1. Provide a large interactional space that can support flexible group working（提供大型交互空间以支持灵活的小组工作）。
2. Can be used by multiple users（可以被多个用户使用）。
3. Can point to and touch information being displayed（可以指向和触摸显示的信息）。
4. Simultaneously view the interactions and have the same shared point of reference as others（同时查看交互并拥有与他人相同的共享参考点）。
5. Can support more equitable participation compared with groups using single PC（与使用单个PC的小组相比，可以支持更公平的参与）。

#### 3.1.14.1 需要考虑的因素
设计共享界面时，需要考虑显示界面的物理特性（如大小、方向和形状）如何影响用户之间的协作。
水平放置的交互表面（如桌子）比垂直表面（如墙壁）更有利于用户之间的互动和协作。
仅仅增加交互表面的尺寸并不能直接提高团队的工作效率，而是可能促进用户之间的任务分工。
提供个人工作区域和共享工作区域可以满足用户在独立工作和团队协作之间的不同需求。
为了支持用户在个人和共享工作空间之间无缝切换，已经开发了跨设备系统。
例如：Surface Constellation，它允许用户在Surface设备之间轻松共享和同步工作。

### 3.1.15 有形界面（Tangible Interfaces）
Type of sensor-based interaction, where physical objects, for example, bricks, are coupled with digital representations（基于传感器的交互类型，其中物理对象（例如砖块）与数字表示相耦合）
When a person manipulates the physical object/s, it causes a digital effect to occur, for example, an animation（当一个人操纵物理对象时，它会引起数字效果的发生，例如，一个动画）
Digital effects can take place in a number of media and places, or they can be embedded in the physical object（数字效果可以在多种媒体和地点发生，或者它们可以嵌入物理对象中）

例子如下：
Urp
Urp是一个交互系统，它允许用户在桌面上移动建筑物的物理模型。
用户可以实际操纵建筑物的模型，这些模型与数字信息相关联。
用户可以使用标记（tokens）来表示风向和阴影等环境因素。
随着时间的推移，系统会在模型周围生成变化的数字阴影，模拟日照效果。
![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/da7b6b1360444f6bace551ce59bbd130.png)

优点：
1. Can be held in one or both hands and combined and manipulated in ways not possible using other interfaces（可以单手或双手持有，并以其他界面无法实现的方式组合和操纵）。
Allows for more than one person to explore the interface together（允许多个人一起探索界面）。
Objects can be placed on top of each other, beside each other, and inside each other（对象可以相互放置、并排或嵌套）。
Encourages different ways of representing and exploring a problem space（鼓励以不同方式表示和探索问题空间）。
2. People are able to see and understand situations differently（人们能够以不同的方式看待和理解情况）。
Can lead to greater insight, learning, and problem-solving than with other kinds of interfaces（比其他类型的界面更能带来更深刻的洞察力、学习能力和解决问题的能力）。
Can facilitate creativity and reflection（可以促进创造力和反思）。
#### 3.1.15.1 需要考虑的因素
设计者需要确定使用哪种概念框架来识别和定义有形界面中独特和具体的特征。

设计者需要考虑用户物理操作和引发的数字反馈之间的关联程度。
如果界面用于支持学习，那么动作和效果之间的明确映射至关重要，以便用户能够理解因果关系。
如果界面用于娱乐，设计可能更倾向于隐性且出人意料，以提供更有趣的体验。

设计者需要决定使用哪种物理对象来与数字内容进行交互。
砖块、立方体和其他组件集因为其灵活性和简单性最常被使用。
棍子和硬纸板令牌也可用于将材料放置在表面上。

设计者需要考虑物理对象与哪些类型的数字输出相结合，例如动画、声音、视觉效果等。

### 3.1.16 增强现实（Augmented Reality）
增强现实技术通过在用户的现实世界视角中叠加计算机生成的图像、视频或其他数字信息，从而“增强”用户的现实体验。
例如：Pokémon Go。
玩家使用智能手机的摄像头和GPS在现实世界中捕捉、战斗和训练虚拟的Pokémon角色，就好像这些角色真的存在于玩家周围的环境中一样。
除了游戏，增强现实技术在多个领域都有广泛的应用。
医学：AR可以帮助医生进行手术模拟、远程诊断或提供实时的解剖信息。
导航：AR可以在用户的现实视野中提供方向指示和信息，帮助他们更轻松地找到目的地。
空中交通管制：AR可以为空中交通管制员提供实时的飞机位置和航线信息，提高管制效率和安全性。
游戏：除了Pokémon Go，还有许多其他AR游戏利用现实环境作为游戏背景，提供独特的游戏体验。
日常探索：AR可以帮助用户在现实世界中发现和探索虚拟信息，如历史遗址的信息叠加、艺术作品的数字标签等。
![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/89b4bf6500254a8ab9428a0c4a7f47e7.png)

#### 3.1.16.1 使用前置摄像头的AR（AR that uses forward facing camera）
前置摄像头可以捕捉用户的脸，然后叠加虚拟物品或效果，如Snapchat的滤镜。
一些零售商店设置了增强现实镜子，顾客可以虚拟试戴化妆品、太阳镜或珠宝。
虚拟试穿技术为顾客提供了一种便捷、互动性强且易于比较不同选择的方式。
尽管虚拟试穿技术提供了便利，但它无法模拟实物的所有感官体验，如重量、质地和气味。
增强现实技术还可以让用户通过前置摄像头“变成”一个特定的角色或名人。
![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/c8321eb975e54f7792575cd26b47a964.png)
![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/9dd179c1986f4fabb59d22ba37ffdbbc.png)
#### 3.1.16.2 需要考虑的因素
设计时需要确定将哪种类型的数字内容叠加到现实世界中。
需要决定数字增强将在何时何地出现在用户的现实环境中。
增强现实的内容需要足够明显，以便用户能够注意到并与之交互，同时又不能过于突兀，以免干扰用户的主要任务。
增强现实的内容需要能够准确地与用户的实际环境对齐，以提供自然的交互体验。
需要考虑如果增强现实的内容与现实环境不完全对齐时会发生什么。
设计时需要考虑目标设备类型，因为不同的设备可能影响AR体验的质量。这包含智能手机、平板电脑、头戴式显示器或其他可穿戴设备等。

### 3.1.17 可穿戴设备（Wearables）
可穿戴技术的早期形式之一是头戴式或眼镜式摄像头，用户可以用它们来记录视野中的内容或获取数字信息。
随着技术的发展，可穿戴设备的形式已经扩展到了各种穿戴物品上。珠宝、头戴式帽子、智能织物、智能眼镜、鞋子和夹克等。
可穿戴设备使得用户能够在移动时方便地访问和操作数字信息。
可穿戴设备被用于多种不同的应用场景，从健康管理到娱乐和时尚。
自动日记：设备可以自动记录用户的活动和体验，如睡眠模式、运动数据等。
旅游指南：可穿戴设备可以提供实时的旅游信息和导航，增强旅行体验。
自行车指示器：为骑行者提供速度、距离和其他骑行相关数据的设备。
时尚服装：结合了智能技术的服装，如可以追踪健康数据或提供其他功能的智能面料。

Google Glass 是一款在2014年发布的增强现实（AR）设备，它通过前置摄像头引发了公众的极大兴奋和关注。然而，这款设备也引起了隐私方面的担忧，特别是关于人们可能在不知情的情况下被拍摄的问题。
![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/5c533e4dc9084133802ea09a39ed6603.png)
#### 3.1.17.1 需要考虑的因素
1. Comfort（舒适性）：
含义：可穿戴设备需要佩戴舒适，不会给用户带来不便。
要求：
轻便：设备需要足够轻，不会给用户造成负担。
小巧：设备体积要小，便于穿戴。
不妨碍：设备设计不能妨碍用户的日常活动。
时尚：外观要时尚，能够融入用户的个人风格。
隐蔽：最好能够隐藏在衣物中，不显眼。
2. Hygiene（卫生）
含义：可穿戴设备需要便于清洁，以保持卫生。
问题：设备或衣物在穿戴后是否能够清洗或清洁。
3. Ease of wear（穿戴便利性）
含义：可穿戴设备需要易于穿戴和脱下。
要求：
易于移除：用户需要能够轻松地移除电子设备。
易于替换：设备需要能够方便地替换或充电。
4. Usability（可用性）
含义：用户需要能够方便地控制嵌入在衣物中的设备。
问题：用户如何与设备交互，例如通过触摸、语音或其他方式

### 3.1.18 机器人（Robots）
在危险环境中使用的远程机器人。例如，可以控制机器人去探测炸弹或其他危险物质，以保护人员安全。
帮助做家务的家用机器人。例如，机器人可以捡起物品或执行吸尘等日常家务。
作为人类伴侣的宠物机器人。它们具有治疗性质，可以帮助减少压力和孤独感。
与人类协作工作的社交机器人。它们鼓励社交行为，可能在教育、医疗或娱乐等领域发挥作用。
例如：Mel和Paro
它们设计得既可爱又令人感到亲切。
可以睁开和闭上眼睛，发出声音和动作。
![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/1f336a22db6d4d389e3a4e67a5aa4f5a.png)
![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/22b373cbb5ef4ae88cd10e0872777d87.png)
再比如无人机。
无人机是一种不需要飞行员在机上的飞行器，可以通过遥控或自主飞行系统进行控制。其被广泛用于各种不同的领域，从娱乐到专业应用。
例如，在节日和聚会上为人们运送饮料和食物。
农业应用，如在葡萄园和田地上空飞行以收集有关作物的数据，这对农民很有用。
帮助在非洲野生动物园追踪偷猎者。
可以低空飞行并将照片传输到地面站，在那里图像可以拼接成地图。
可以用来确定作物的健康状况，或确定最佳的收获时间。
![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/f3f7cf8835a54c07a5e020fde77cf26d.png)
#### 3.1.18.1 需要考虑的因素
研究人们如何与表现出类似人类行为（如面部表情）的物理机器人互动，与虚拟机器人相比有何不同。
设计时需要考虑机器人的外观和行为是否应该模仿人类，或者看起来和行为都像机器人，以清楚地传达其用途。
设计时需要决定交互方式是更像人与人之间的自然交流，还是更像传统的人机交互（如通过按钮或屏幕）。
这涉及到无人机使用的伦理和隐私问题。

### 3.1.19 脑机接口（Brain-computer interfaces）
脑机接口（BCI）提供了一个人脑波与外部设备（如屏幕上的光标）之间的通信路径。
用户需要学习如何通过特定的思维模式来控制BCI设备。
BCI系统通过监测大脑活动的变化来识别用户的意图。
BCI技术可以应用于各种应用程序，提供新的交互方式。
例如：
Games（游戏）：如“Brain Ball”等游戏，用户可以通过思维控制游戏中的角色或元素。
Enable people who are paralyzed to control robots（使瘫痪的人能够控制机器人）：BCI可以帮助那些因疾病或伤害而无法移动的人通过思考来控制轮椅、假肢或其他辅助设备。

下图展示了一位瘫痪的女性使用脑机接口在屏幕上选择字母。
![在这里插入图片描述](https://i-blog.csdnimg.cn/direct/0f868138b32448abbe7046fa6582093a.png)

### 3.1.20 智能界面（Smart interfaces）
智能界面可以应用于各种设备和环境中，如个人电子设备（手机、扬声器、手表）、交通工具（汽车）、住宅和城市基础设施。
智能界面不仅仅是自动化的，它们还具备一定的智能，能够通过互联网连接到其他设备和服务。
智能界面能够感知和理解周围环境的情况，并根据这些信息执行适当的动作。
智能建筑被设计为能够感知居住者的需求并代表他们采取行动，同时也允许居住者与自动化系统进行一定程度的控制和互动。

## 3.2 选择哪种界面？
使用哪种界面将取决于任务、用户、上下文、成本、鲁棒性等。
在特定环境中，多媒体界面（结合多种媒体形式，如视频、音频和文本）是否比有形界面（涉及物理对象和直接操作）更有效。
我们还可以比较语音界面（使用语音命令和识别）和基于命令的界面（使用文本或按钮输入命令）在执行任务时的有效性。
多模态界面是否提供更好的用户体验和效率。
可穿戴界面是否比移动界面更有助于人们在外国城市中查找信息。
虚拟环境是否是玩游戏的最终界面。
与使用联网的台式电脑相比，可共享界面是否更擅长支持通信和协作。