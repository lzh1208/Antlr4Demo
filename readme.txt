在idea下使用antlr解析的步骤
1.编写对应语法的g4文件
2.右键要翻译的的g4文件，首先Configure ANTLR,指定生成文件的路径
  主要在“Output directory where all output id generated”指定主路径（一直到*src/java目录）
  然后在“Package/namespace for the generated code”指定项目的详细路径
  注意勾选，generate phrase tree listener(default) 和generate phrase tree visitor
3.右键要翻译的g4文件，选择Generate ANTLR Recognizer,这样就会生成对应的文件
4.编写解析器功能代码，运行代码

注意：请确保安装插件 ANTLR v4 grammar plugin，可以在idea插件库自动下载
