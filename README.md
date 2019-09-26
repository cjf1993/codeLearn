# codeLearn

Eclipse在新建项目的时候会自动生成一些文件。
这些文件比如.project、.classpath、.settings目录下的所有文件等。
这些文件是Eclipse项目的元数据，描述了一个Eclipse项目。

Eclipse项目根目录下通常有两个文件：.project和.classpath，
.project是Eclipse项目必须有的文件，
而.classpath是Java项目必须有的文件。这两个文件均是XML格式的文本文件，用普通文本编辑器即可打开。

.project描述了一个Eclipse项目。
.classpath描述了一个Eclipse项目。
.jsdtscope文件定义了web项目中的源码路径，也就意味着只有web project才会有这个配置。这些源码Eclipse会进行validate（如果validate没有禁用）。这个文件在实际开发中最大的价值在于定义JS文件的例外路径，在配置界面中配置的话挨个选很烦人。
.org.eclipse.core.resources.prefs文件其实就是规定项目内的文件的编码用的。一般来说一个项目里的文件编码需要一致，特别是文件文本内容本身无法指示文件本身编码的（比较绕，XML文件第一行能指示自身编码，CSS也有这个能力但用得不多），尽量不要多种编码同时存在（最好在编码规范中禁止多重编码同时存在的现象发生）。
.org.eclipse.jdt.core.prefs文件指定了一些Java编译的特性，比如Java版本之类的，看文件每一行的key能猜出具体的用处。
.org.eclipse.m2e.core.prefs是一些maven相关的配置。
.org.eclipse.wst.common.component文件规定了项目怎么组装成一个webapp，这里可以玩很多种组装方式。
.org.eclipse.wst.common.project.facet.core.xml指示了项目中启用那些facet及facet的版本。
