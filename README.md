#An efficient web framework
#一個高效的web框架
##为什么高效
###1.异步请求
###2.异步写入数据库


##安全验证
####1.请使用如下方法操作cookie：
self.set_secure_cookie，
self.get_secure_cookie
####2.敏感操作请使用post，添加_xsrf字段防止xsrf攻击
##请求处理
####1.避免使用同步操作
####2.请求处理流程：init-->handler-->control-->db
##数据库操作
####1.大批量的插入、删除、更新建议使用原生sql，速度会提高一倍，详情参考test_sqlalchemy.py
####2.异步操作mysql，详情查看test下sync_mysql.py

