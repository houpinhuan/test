# test
2018.11.20
Git版本控制
的
git 拉取项目：git clone git地址
上传代码
更新代码  
1.git  status 查看是否冲突
2.git pull 更新语句
3.cd到你的项目目录 :$ cd /Users/cjk/Desktop/myShop
4.然后,输入git命令: $ git init  
5.将项目的所有文件添加到缓存中:$ git add . 
6.将缓存中的文件Commit到git库: $ git commit -m "添加你的注释,备注"

laravel打印sql语句
echo Stylist::where($where)->toSql();
echo Stylist::toSql();

2018.11.21
laravel 打印简单数组格式，不含复杂的格式
echo "<pre>";
print_r($data->toarray());
echo "<pre>";

laravel  多个求和sum
$data = Stylist::
        select(DB::raw('count(status) as c'),'status',DB::raw('sum(userId) as s'))
        ->groupBy('status')
        ->get();
