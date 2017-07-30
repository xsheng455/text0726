# 流行框架
## ssh方式上传代码
1. 生成公钥和私钥
    * ssh-keygen -t rsa -C "youxinag"
2. 在用户目录下.ssh 中复制..pub文件内容，在GitHub中用户下找settings找ssh and g.. 点击新秘钥

## 下载
1. git pull ssh地址 master

## 处理冲突
   本地与服务器端的代码发生冲突时，根据需要删除不需要的代码

## 提交数据时先pull再push
    先pull时，如果服务器版本和本地不同，我们可以把冲突先解决，然后把最新的版本push到服务器
##  简写
    git remote add 变量 地址 
    git push 变量 -u master
    当我们在push时，加上了-u参数，那么下一次push时只需要写git push 就能上传代码了；

## npm 使用 （node package manage）
1. 新建文件夹 右键运行 npm init 一路回车，会生成一个package.json 文件
2. npm install jQuery 会去下载jQuery
3. npm install jQuery --save 会在json文件中添加当前下载包的版本信息
4. cnpm 淘宝镜像
5. npm install 会下载json目录下的插件
npm install cnpm -g --registry=https://registry.npm.taobao.org

## 5个核心方法
1. gulp.task('任务名',function(){})//创建任务
2. gulp.src('./*'.css)//指定想要处理的文件
3. gulp.dest()//指定最终处理后的文件的存放路径
4. gulp.watch() // 自动的监视文件的变化，然后执行相应任务。
5. gulp.run('任务名')，直接执行相应的任务。

##  gulp 的安装与使用
    通过npm安装:npm install gulp-cli -g
1.  在当前项目中也要安装gulp: `npm install gulp --save`
2. 还需要在当前项目中新建一个文件: gulpfile.js

var gulp=require("gulp");
gulp.task("test",function(){
    console.log(1234);
});

使用:gulp test(任务名);

gulp.task("con",function(){
    gulp.src(["./one.js","./two.js","./three.js"])
    .pipe(concat("./index-min.js"))
    .pipe(uglify())
    .pipe(gulp.dest("./dist"))
})

## 对css进行压缩操作
 `npm install gulp-cssnano --save`
// 新建一个任务，对css进行处理
gulp.task('style', function(){
  // 对项目中的2个css文件进行合并，压缩操作
  // 1.匹配到要处理的文件
  gulp.src(['./*.css'])
  // 2.合并文件
  .pipe(concat('index.css'))
  // 3.压缩操作
  .pipe(cssnano())
  // 4.输出到指定目录
  .pipe(gulp.dest('./dist'))
  })

### 对html进行压缩
- `npm install gulp-htmlmin --save`
- https://github.com/kangax/html-minifier



















