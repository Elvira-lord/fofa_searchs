# fofa_searchs
批量进行fofa语句的搜索+批量探活+轻量指纹

这个目录下一定要有个文件夹 result ，不然会报错，这里是存储结果文件的地方
<img width="1535" height="740" alt="image" src="https://github.com/user-attachments/assets/4beec660-c4b9-4490-9e68-56c448436c93" />

结果会自动保存在 result.xlsx 文件中
<img width="1650" height="734" alt="image" src="https://github.com/user-attachments/assets/db966305-64da-493e-ba4b-11e7d462ec41" />
<img width="1721" height="743" alt="image" src="https://github.com/user-attachments/assets/bf8444f9-885c-4638-b27b-b6f84a65a103" />


config.ini 设置调整
一些卖fofa的url可能是类似 fofa.icu 这种的，直接更改文件 config.ini 文件中的 fofa_url='https://fofa.icu'
是否保存在同一个文件，默认  is_save_the_file:True  这里是 True ，改为 False 则在result里面批量创建文件，命名以每次fofa的搜索语法中第一个 "" 或者 ''
file_name='result.xlsx'  这里保存在同一个文件夹中的文件
[0,200, 302, 404, 500]  分类的sheet，可根据需求填写，格式不变
size=100  每次查询的数量，这里默认 100 ，可自行调整

执行文件第 365 行为线程数，默认为20
    max_workers = 20  #并发线程数


