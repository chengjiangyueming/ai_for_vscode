# 在VS Code 里使用
## 步骤
### 准备
- 用chromium内核的浏览器（chrome,edge...)
- 安装[vscode](https://code.visualstudio.com/)
	- 工作环境
- 安装[steam++](https://steampp.net/)
	- 修改DNS，避免污染
- 安装claude code到本地
	- 先打开steam++，进行github加速
	- Bing搜索到这个网址[claude安装文档](https://code.claude.com/docs/en/overview)
	- 选择对应安装方式
		- windows用winget可以不用科学上网
	- 打开shell安装，安装成功后配置API key
	- deepseek配置代码在deepseek[接口文档](https://api-docs.deepseek.com/zh-cn/quick_start/agent_integrations/claude_code)
	- 安装cc swith，[官网](https://www.ccswitch.io/zh/)
	- 打开cc swith,如果defeat有模型，说明配置很成功，你的网络环境应该很好。没有也不用担心，点击+号添加模型deepseek或者其他 
- 获取API key
	- 打开[deepseek API 平台](https://platform.deepseek.com/)
	- 获取API key,可以先预充值也可以不用
	- 其他ai的获取大同小异
- 注册github
	- 保持steam++后台运行，登录[github官网](https://github.com/)注册
- 准备完成
### vscode配置
- 先完成github登录，python环境，简体中文，csv显示，pdf显示等基础内容
- 这里你就可以使用coplit了，但是不建议使用，这个的命中率不高，想尝鲜的也可以试试。不想用的找到右下的coplit兔子图标和右上的智能体中心，将其全部禁用。
- 通过插件市场安装cline（第一个）拓展
	- 点击打开后，选第三个（用自己的api),然后在对应输入框输入api key,勾选分别配置选项框，plan用Pro模型，act用flash
	- 点击cline设置，找到扳手（总设置）设置为简中，重启
- 以同样的方式安装claude code拓展，然后claude不需额外配置，因为已经配置在本地了![屏幕截图 2026-06-24 215747 1](attachment/屏幕截图%202026-06-24%20215747%20.png)
- 现在左侧边框有一个机器人图标（cline),花瓣图标（claude）；右下标签栏内有一个兔子机器人图标（coplit)![屏幕截图 2026-06-24 220129](attachment/屏幕截图%202026-06-24%20220129.png)
- claude 可以右键永久布局到右侧栏
- 最后安装jupyter拓展，vscode会提示你发现新大陆
- 配置完成
### 运用
- 打开一个你需要工作的文件夹
- 新建文件，选择jupyter notebook,新建了一个.ipynb文件![屏幕截图 2026-06-24 215855 1](attachment/屏幕截图%202026-06-24%20215855%20.png)
- 选择内核连接到python，你可以先输入一个`print("hello world")`,按步骤点击，最后,会弹出错误，根据提示进入shell安装
- 现在可以进行你的思考和编译了
	- 遇到没有灵感或者报错，可以点击右键键入claude或者点击💡键入cline，或者你还没有禁用coplit，它会直接给你一个预设修改让你tab键入直接修改
- 编译后你需要的输出，可以有的至少几个选择，均在claude里使用
	- 输出csv，你的提示词大概是对文件夹内已有csv进行整合
	- 输出word或者pdf,你的提示词大概是根据我给你的参考模板文件进行格式复制。如果你是latex，可能需要你额外有其他解释器和转换器如texlive+pandoc
	- 输出PPT,你的提示词大概是生成ppt或者先生成html后生成ppt
		- 注意，PPT 内的样式如果是你不提供模板或者元素，会使用svg伪元素，效果可能不佳
	- ==最后重要的是==，如果你不想ai给你生成文档，请让他生成txt或者obsidian cli的原生markdown。==介意的点==可能是如果让ai生成docx,xlsx,pptx会是==兼容模式==，需要你全选复制，在另一个新文档里粘贴==源格式==。当然，使用txt或者obsidian cli原生markdown就很不错了
### 推荐
- 不要放过这个Leo老师，XXHK（学习骇客）公众号，最新的课程可以蹲一蹲
- 强烈建议使用参考文献和论文处理使用热门的obsidian+claudian插件进行管理和学习
- claude你至少应该在社区下载skills有两个create-skills和find-skills，可以补齐deepseek除了识图以外的所有短板
