# Algorithm_Template

NENU LosWin Algorithm Template

弱队整理的不完备（可能也不靠谱）的 算法模板 一份

可能没有精力再维护了，有需要的同学可以拿去用（或者在此基础上组织一份自己的模板）

算法竞赛再见

关于接下来维护的一些小建议：

 - 利用 \lstinputlisting 指令将当前单纯的 \lstlisting 部分替换，将 cpp/java 代码文件与 tex 文件分离，方便查询与修改。\lstinputlisting 指令示例： \lstinputlisting[language=C++, title=test.cpp]{test.cpp}，个人建议实现一个脚本去完成修改操作（手动搞工作量有点离谱

 - 一些简单易于默写的基础算法的代码并没有加入模板内，可以根据需要添加

 - 由于模板整理的总过程近四年，所以代码风格可能变来变去，可以根据需要统一整理

 - 代码块字体配色方案等格式可以自行设置，下面是用过的两种代码块格式

基础版本
```tex
% 代码块格式设置
\lstset{
    breaklines = true,                  % 让 LaTeX 自动将长的代码行换行排版
    extendedchars = false,              % 解决代码跨页时，章节标题，页眉等汉字不显示的问题
    basicstyle = \sffamily,             % 基本代码风格
    keywordstyle = \bfseries,           % 关键字风格
    commentstyle = \rmfamily\itshape,   % 注释的风格，斜体
    stringstyle = \ttfamily,            % 字符串风格
    columns = fixed,                    % 如果不加这一句，字间距就不固定，很丑，必须加
    numbers = left,                     % 行号的位置在左边
    showspaces = false,                 % 是否显示空格，显示了有点乱，所以不现实了
    numberstyle = \zihao{-5}\ttfamily,  % 行号的样式，小五号，tt 等宽字体
    showstringspaces = false,
    captionpos = t,                     % 这段代码的名字所呈现的位置，t 指的是 top 上面
    frame = lrtb,                       % 显示边框
}
```

微软雅黑，代码高亮
```tex
% 代码块格式设置
\lstset{
    breaklines = true,                                          % 让 LaTeX 自动将长的代码行换行排版
    extendedchars = false,                                      % 解决代码跨页时，章节标题，页眉等汉字不显示的问题
    columns = fixed,                                            % 如果不加这一句，字间距就不固定，很丑，必须加
    numbers = left,                                             % 行号的位置在左边
    showspaces = false,                                         % 是否显示空格，显示了有点乱，所以不现实了
    numberstyle = \zihao{-5} \ttfamily,                         % 行号的样式，小五号，tt 等宽字体
    showstringspaces = false,
    captionpos = t,                                             % 这段代码的名字所呈现的位置，t 指的是 top 上面
    frame = lrtb,                                               % 显示边框
    morekeywords = {alignas,continute,friend,register,true,alignof,decltype,goto,
    reinterpret_cast,try,asm,defult,if,return,typedef,auto,delete,inline,short,
    typeid,bool,do,int,signed,typename,break,double,long,sizeof,union,case,
    dynamic_cast,mutable,static,unsigned,catch,else,namespace,static_assert,using,
    char,enum,new,static_cast,virtual,char16_t,char32_t,explict,noexcept,struct,
    void,export,nullptr,switch,volatile,class,extern,operator,template,wchar_t,
    const,false,private,this,while,constexpr,float,protected,thread_local,
    const_cast,for,public,throw,std},
    basicstyle = \fontspec{Courier New},                                        % 基本代码风格
    keywordstyle = \fontspec{Courier New Bold} \color[RGB]{64, 64, 255},        % 关键字风格
    commentstyle = \fontspec{Courier New Italic} \color[RGB]{128, 128, 128},      % 注释的风格
    stringstyle = \fontspec{Courier New Italic} \color[RGB]{128, 0, 0},         % 字符串风格
    % basicstyle = \fontspec{Courier New Bold},
    % basicstyle = \fontspec{Consolas},
    % basicstyle = \fontspec{微软雅黑},
}
```


