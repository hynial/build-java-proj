自定义组建java项目shell脚本，存位于/usr/bin/bjpro
使用操作：(新建一个文件夹命名为项目名称，即项目根目录)
1、进入初始化项目根目录，编辑文件compile，根据文件末尾操作
2、写好你的代码于src目录，包文件放于src/lib目录
3、切换到项目根目录，编译你的java项目：./compile
4、不出错就进入classes/Onserver目录，编辑run文件，写好你的运行配置，依赖jar包等信息
5、切换到Onserver目录，运行run文件：./run
6、不出错就可以看到运行结果
打包jar操作：
1、编辑classes下的manifest.mf文件，填好相关信息，主类依赖jar包等信息
2、切换到Onserver目录，运行：jar cvmf ../manifest.mf 自定义jar文件名.jar .
3、不出错当前目录下生成文件：自定义jar文件名.jar
4、试试运行jar包：java -jar 自定义jar文件名.jar

因为升级了XCode 出现requires admin privileges问题，解决方法是：
sudo xcodebuild -license
while(1) 'space';agree 
