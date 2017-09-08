# workRecord
记录自己的工作问题

## eclipse出现An internal error occurred during: "Building workspace". Java heap space 错误。##

出现这个错误，eclipse 会卡死，以及自动退出
解决方案 
工程根目录 找到项目中.project文件
删除这两处
  第一处：
 <pre><code> <buildCommand>
         <name>org.eclipse.wst.jsdt.core.javascriptValidator</name>
         <arguments>
         </arguments>
	<ildCommand>
</code></pre>
第二处：
 pre><code><nature>org.eclipse.wst.jsdt.core.jsNature</nature></pre>
