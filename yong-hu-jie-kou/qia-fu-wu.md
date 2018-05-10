# 卡服务 #
 
************************
************************
### 1 商户银行卡列表查询 ###

#### 1.1接口描述 ####

查询商户银行卡列表信息。

#### 1.2接口概述 ####
##### 接口类：#####
<pre>
com.suixingpay.icp.ums.dubbo.bank.UmsStmBankCardQueryDubbo
</pre>
##### 接口方法名：#####
<pre>
queryStmBankCardByUuid    
</pre>
##### 输入业务参数类型： #####
<pre>
com.suixingpay.common.rpc.v2.RpcRequest< QueryUsrStmBnkRequest >
</pre>
##### 输出业务参数类型： #####
<pre>
com.suixingpay.common.rpc.v2.RpcResponse< ResponseMsgStmBnk >
</pre>


#### 1.3 参数说明 ####
##### 输入参数： #####

字段名称 | 类型 | 输入项 | 备注
---|---|---|---
uuid | String | 空 | 请求流水ID
sysId | String | 非空 | 系统编码
object | QueryUsrStmBnkRequest | 非空 | 业务参数

QueryUsrStmBnkRequest：

字段名称 | 类型 | 输入项 | 备注
---|---|---|---
uuid| String | 非空 | 商户号


##### 响应参数： #####

字段名称 | 类型 | 输入项 | 备注
---|---|---|---
code | String | 非空 | 返回码
message | String | 非空 | 返回信息
object | ResponseMsgStmBnk | 非空 | 业务参数

ResponseMsgStmBnk < listReturn >：

字段名称 | 类型 | 输入项 | 备注
---|---|---|---
xx| String | 非空 | 银行卡类型
xx| String | 非空 | 卡号 
xx| String | 非空 | 户名
xx| String | 非空 | 开户银行
xx| String | 非空 | 联行名称
xx| String | 非空 | 联行号
xx| String | 非空 | 绑定时间
xx| String | 非空 | 是否默认结算卡


#### 1.4响应码说明 ####

code | 描述
---|---
0000| 成功
999999| 系统异常

************************

### 2 商户银行卡添加接口###

#### 2.1接口描述 ####

添加商户银行卡信息。

#### 2.2接口概述 ####
##### 接口类： #####
<pre>
com.suixingpay.icp.ums.dubbo.bank.UmsStmBankCardDubbo
</pre>
##### 接口方法名： #####
<pre>
addUsrStmBnk  
</pre>
##### 输入业务参数类型： #####
<pre>
com.suixingpay.common.rpc.v2.RpcRequest< BapAddUsrStmBnkRequest >
</pre>
##### 输出业务参数类型： #####
<pre>
com.suixingpay.common.rpc.v2.RpcResponse< BapAddUsrStmBnkResponse >
</pre>


#### 2.3 参数说明 ####
##### 输入参数： #####

字段名称 | 类型 | 输入项 | 备注
---|---|---|---
uuid | String | 非空 | 请求流水ID
sysId | String | 非空 | 系统编码
object | BapAddUsrStmBnkRequest | 非空 | 业务参数

BapAddUsrStmBnkRequest：

字段名称 | 类型 | 输入项 | 备注
---|---|---|---
defaultFlg| String | 非空 | 结转账户标识
actTyp| String | 非空 | 银行卡账户类型
usrId| String | 非空 | 用户号
actNo| String | 非空 | 银行卡账户号
actNm| String | 非空 | 银行卡账户户名
lbnkProv| String | 非空 | 开户行所在省编码
lbnkCity| String | 非空 | 开户行所在市编码
bnkCd| String | 非空 | 开户银行编码
lbnkNo| String | 非空 | 开户银行行号
lbnkNm| String | 非空 | 开户银行名称


##### 响应参数： #####

字段名称 | 类型 | 输入项 | 备注
---|---|---|---
code | String | 非空 | 返回码
message | String | 非空 | 返回信息
object | BapAddUsrStmBnkResponse | 非空 | 业务参数

BapAddUsrStmBnkResponse：

字段名称 | 类型 | 输入项 | 备注
---|---|---|---
uuid| String | 非空 | 卡信息ID


#### 2.4响应码说明 ####

code | 描述
---|---
0| 成功
999999| 系统异常


************************

### 3 商户银行卡修改接口###

#### 3.1接口描述 ####

修改商户银行卡信息。

#### 3.2接口概述 ####
##### 接口类： #####
<pre>
com.suixingpay.icp.ums.dubbo.bank.UmsStmBankCardDubbo
</pre>
##### 接口方法名： #####
<pre>
updateUsrStmBnk  
</pre>
##### 输入业务参数类型： #####
<pre>
com.suixingpay.common.rpc.v2.RpcRequest< BapUpdateUsrStmBnkRequest >
</pre>
##### 输出业务参数类型： #####
<pre>
com.suixingpay.common.rpc.v2.RpcResponse< BapUpdateUsrStmBnkResponse >
</pre>


#### 3.3 参数说明 ####
##### 输入参数： #####

字段名称 | 类型 | 输入项 | 备注
---|---|---|---
uuid | String | 非空 | 请求流水ID
sysId | String | 非空 | 系统编码
object | BapAddUsrStmBnkRequest | 非空 | 业务参数

BapAddUsrStmBnkRequest：

字段名称 | 类型 | 输入项 | 备注
---|---|---|---
defaultFlg| String | 非空 | 结转账户标识
actTyp| String | 非空 | 银行卡账户类型
usrId| String | 空 | 用户号
actNo| String | 非空 | 银行卡账户号
actNm| String | 非空 | 银行卡账户户名
lbnkProv| String | 非空 | 开户行所在省编码
lbnkCity| String | 非空 | 开户行所在市编码
bnkCd| String | 非空 | 开户银行编码
lbnkNo| String | 非空 | 开户银行行号
lbnkNm| String | 非空 | 开户银行名称
OrnOrdNo| String | 空 | 幂等参数
uuid| String | 空 | 卡信息ID
actSts| String | 非空 | 状态


##### 响应参数： #####

字段名称 | 类型 | 输入项 | 备注
---|---|---|---
code | String | 非空 | 返回码
message | String | 非空 | 返回信息
object | BapUpdateUsrStmBnkResponse | 非空 | 业务参数

BapUpdateUsrStmBnkResponse：

字段名称 | 类型 | 输入项 | 备注
---|---|---|---
uuid| String | 非空 | 卡信息ID


#### 3.4响应码说明 ####

code | 描述
---|---
0| 成功
999999| 系统异常

************************


### 4 商户银行卡删除接口###

#### 4.1接口描述 ####

删除商户银行卡信息。

#### 4.2接口概述 ####
##### 接口类： #####
<pre>
com.suixingpay.icp.ums.dubbo.bank.UmsStmBankCardDubbo
</pre>
##### 接口方法名： #####
<pre>
deleteUsrStmBnk  
</pre>
##### 输入业务参数类型： #####
<pre>
com.suixingpay.common.rpc.v2.RpcRequest< BapDeleteUsrStmBnkRequest >
</pre>
##### 输出业务参数类型： #####
<pre>
com.suixingpay.common.rpc.v2.RpcResponse< BapDeleteUsrStmBnkResponse >
</pre>


#### 4.3 参数说明 ####
##### 输入参数： #####

字段名称 | 类型 | 输入项 | 备注
---|---|---|---
uuid | String | 非空 | 请求流水ID
sysId | String | 非空 | 系统编码
object | BapAddUsrStmBnkRequest | 非空 | 业务参数

BapDeleteUsrStmBnkRequest：

字段名称 | 类型 | 输入项 | 备注
---|---|---|---
inMno| String | 非空 | 内编
actNo| String | 非空 | 银行卡账户号
ornOrdNo| String | 非空 | 幂等参数
uuid| String | 非空 | 主键
usrId| String | 非空 | 用户Id
defaultFlg| String | 非空 | 默认标识


##### 响应参数： #####

字段名称 | 类型 | 输入项 | 备注
---|---|---|---
code | String | 非空 | 返回码
message | String | 非空 | 返回信息
object | BapDeleteUsrStmBnkResponse | 非空 | 业务参数

BapDeleteUsrStmBnkResponse：

字段名称 | 类型 | 输入项 | 备注
---|---|---|---



#### 4.4响应码说明 ####

code | 描述
---|---
0| 成功
999999| 系统异常


************************


### 5 商户银行卡设置默认结算卡接口###

#### 5.1接口描述 ####

设置商户银行卡为默认结算卡信息。

#### 5.2接口概述 ####
##### 接口类： #####
<pre>
com.suixingpay.icp.ums.dubbo.bank.UmsStmBankCardDubbo
</pre>
##### 接口方法名： #####
<pre>
setDefaultStmAcct  
</pre>
##### 输入业务参数类型： #####
<pre>
com.suixingpay.common.rpc.v2.RpcRequest< BapUsrStmBnkDefAccRequest >
</pre>
##### 输出业务参数类型： #####
<pre>
com.suixingpay.common.rpc.v2.RpcResponse< BapUsrStmBnkDefAccResponse >
</pre>


#### 5.3 参数说明 ####
##### 输入参数： #####

字段名称 | 类型 | 输入项 | 备注
---|---|---|---
uuid | String | 非空 | 请求流水ID
sysId | String | 非空 | 系统编码
object | BapUsrStmBnkDefAccRequest | 非空 | 业务参数

BapUsrStmBnkDefAccRequest：

字段名称 | 类型 | 输入项 | 备注
---|---|---|---
inMno| String | 非空 | 内编
actNo| String | 非空 | 银行卡账户号
ornOrdNo| String | 非空 | 幂等参数
uuid| String | 非空 | 主键
sysId| String | 空 | 系统来源
defaultFlg| String | 非空 | 结转标识


##### 响应参数： #####

字段名称 | 类型 | 输入项 | 备注
---|---|---|---
code | String | 非空 | 返回码
message | String | 非空 | 返回信息
object | BapUsrStmBnkDefAccResponse | 非空 | 业务参数

BapUsrStmBnkDefAccResponse：

字段名称 | 类型 | 输入项 | 备注
---|---|---|---



#### 5.4响应码说明 ####

code | 描述
---|---
0| 成功
999999| 系统异常

