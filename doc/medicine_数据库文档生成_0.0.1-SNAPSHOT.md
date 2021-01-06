# 医药器材进销存管理系统的设计与实现

**数据库名：** medicine

**文档版本：** 0.0.1-SNAPSHOT

**文档描述：** 数据库文档生成
| 表名                  | 说明       |
| :-------------------- | :--------- |
| [admin](#admin) |  |
| [allorder](#allorder) |  |
| [aprecord](#aprecord) |  |
| [orderdetails](#orderdetails) |  |
| [product](#product) |  |
| [repertory](#repertory) |  |
| [shoukuan](#shoukuan) |  |
| [warehouse](#warehouse) |  |
**表名：** <a id="admin">admin</a>

**说明：** 

**数据列：**

| 序号 | 名称 | 数据类型 |  长度  | 小数位 | 允许空值 | 主键 | 默认值 | 说明 |
| :--: | :--- | :------: | :----: | :----: | :------: | :--: | :----: | :--: |
|  1   | admin_username |   varchar   | 255 |   0    |    N     |  Y   |       |   |
|  2   | admin_password |   varchar   | 255 |   0    |    N     |  N   |       |   |
|  3   | admin_name |   varchar   | 255 |   0    |    Y     |  N   |       |   |
**表名：** <a id="allorder">allorder</a>

**说明：** 

**数据列：**

| 序号 | 名称 | 数据类型 |  长度  | 小数位 | 允许空值 | 主键 | 默认值 | 说明 |
| :--: | :--- | :------: | :----: | :----: | :------: | :--: | :----: | :--: |
|  1   | order_odid |   int   | 10 |   0    |    N     |  Y   |       |   |
|  2   | order_allmoney |   int   | 10 |   0    |    Y     |  N   |       |   |
|  3   | order_status |   varchar   | 255 |   0    |    Y     |  N   |       |   |
|  4   | order_time |   datetime   | 19 |   0    |    Y     |  N   |       |   |
**表名：** <a id="aprecord">aprecord</a>

**说明：** 

**数据列：**

| 序号 | 名称 | 数据类型 |  长度  | 小数位 | 允许空值 | 主键 | 默认值 | 说明 |
| :--: | :--- | :------: | :----: | :----: | :------: | :--: | :----: | :--: |
|  1   | ausername |   varchar   | 255 |   0    |    N     |  N   |       |   |
|  2   | pid |   int   | 10 |   0    |    N     |  N   |       |   |
|  3   | num |   int   | 10 |   0    |    N     |  N   |       |   |
|  4   | time |   datetime   | 19 |   0    |    Y     |  N   |       |   |
**表名：** <a id="orderdetails">orderdetails</a>

**说明：** 

**数据列：**

| 序号 | 名称 | 数据类型 |  长度  | 小数位 | 允许空值 | 主键 | 默认值 | 说明 |
| :--: | :--- | :------: | :----: | :----: | :------: | :--: | :----: | :--: |
|  1   | orderdetails_id |   int   | 10 |   0    |    N     |  N   |       |   |
|  2   | orderdetails_pid |   int   | 10 |   0    |    Y     |  N   |       |   |
|  3   | orderdetails_wid |   int   | 10 |   0    |    Y     |  N   |       |   |
|  4   | orderdetails_price |   int   | 10 |   0    |    Y     |  N   |       |   |
|  5   | orderdetails_num |   int   | 10 |   0    |    Y     |  N   |       |   |
|  6   | orderdetails_time |   datetime   | 19 |   0    |    Y     |  N   |       |   |
**表名：** <a id="product">product</a>

**说明：** 

**数据列：**

| 序号 | 名称 | 数据类型 |  长度  | 小数位 | 允许空值 | 主键 | 默认值 | 说明 |
| :--: | :--- | :------: | :----: | :----: | :------: | :--: | :----: | :--: |
|  1   | product_id |   int   | 10 |   0    |    N     |  Y   |       |   |
|  2   | product_name |   varchar   | 255 |   0    |    Y     |  N   |       |   |
|  3   | product_producer |   varchar   | 255 |   0    |    Y     |  N   |       |   |
|  4   | product_price |   int   | 10 |   0    |    Y     |  N   |       |   |
**表名：** <a id="repertory">repertory</a>

**说明：** 

**数据列：**

| 序号 | 名称 | 数据类型 |  长度  | 小数位 | 允许空值 | 主键 | 默认值 | 说明 |
| :--: | :--- | :------: | :----: | :----: | :------: | :--: | :----: | :--: |
|  1   | repertory_wid |   int   | 10 |   0    |    N     |  N   |       |   |
|  2   | repertory_pid |   int   | 10 |   0    |    N     |  N   |       |   |
|  3   | repertory_stime |   datetime   | 19 |   0    |    Y     |  N   |       |   |
|  4   | repertory_num |   int   | 10 |   0    |    Y     |  N   |       |   |
**表名：** <a id="shoukuan">shoukuan</a>

**说明：** 

**数据列：**

| 序号 | 名称 | 数据类型 |  长度  | 小数位 | 允许空值 | 主键 | 默认值 | 说明 |
| :--: | :--- | :------: | :----: | :----: | :------: | :--: | :----: | :--: |
|  1   | shoukuan_admin |   varchar   | 255 |   0    |    Y     |  N   |       |   |
|  2   | shoukuan_money |   int   | 10 |   0    |    Y     |  N   |       |   |
|  3   | shoukuan_time |   datetime   | 19 |   0    |    Y     |  N   |       |   |
**表名：** <a id="warehouse">warehouse</a>

**说明：** 

**数据列：**

| 序号 | 名称 | 数据类型 |  长度  | 小数位 | 允许空值 | 主键 | 默认值 | 说明 |
| :--: | :--- | :------: | :----: | :----: | :------: | :--: | :----: | :--: |
|  1   | warehouse_id |   int   | 10 |   0    |    N     |  Y   |       |   |
|  2   | warehouse_address |   varchar   | 255 |   0    |    Y     |  N   |       |   |
|  3   | warehouse_name |   varchar   | 255 |   0    |    Y     |  N   |       |   |
|  4   | warehouse_admin |   varchar   | 255 |   0    |    Y     |  N   |       |   |
