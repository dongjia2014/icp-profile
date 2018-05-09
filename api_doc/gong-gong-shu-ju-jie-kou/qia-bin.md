# 卡BIN #
 
************************
### 1 卡bin匹配查询接口###

#### 1.1接口描述 ####

通过传入的卡号进行卡bin查询匹配，返回相应查询信息。

#### 1.2接口概述 ####
##### 接口类： #####
<pre>
com.suixingpay.bap.api.ses.SesCardBinQueryDubbo
</pre>
##### 接口方法名： #####
<pre>
crdBinQry    
</pre>
##### 输入业务参数类型： #####
<pre>
com.suixingpay.common.rpc.v2.RpcRequest< SesBnkCardBinInfoReq >
商户信息Bean
</pre>
##### 输出业务参数类型： #####
<pre>
com.suixingpay.common.rpc.v2.RpcResponse< SesBnkCardBinInfoRsp >
商户信息Bean
</pre>


#### 1.3 参数说明 ####
##### 输入参数： #####

字段名称 | 类型 | 输入项 | 备注
---|---|---|---
uuid | String | 空 | 请求流水ID
sysId | String | 非空 | 系统编码
object | SesBnkCardBinInfo | 非空 | 业务参数

SesBnkCardBinInfo：

字段名称 | 类型 | 输入项 | 备注
---|---|---|---
qryCardNo| String | 非空 | 查询卡号


##### 响应参数： #####

字段名称 | 类型 | 输入项 | 备注
---|---|---|---
uuid | String | 空 | 请求流水ID
sysId | String | 非空 | 系统编码
object | SesBnkCardBinInfo | 非空 | 业务参数

SesBnkCardBinInfo：

字段名称 | 类型 | 输入项 | 备注
---|---|---|---
qryCardNo| String | 非空 | 查询卡号
bnkNm| String | 非空 | 发卡行名称
bnkBnm| String | 非空 | 发卡行行别
bnkBno| String | 非空 | 银行机构代码
isInBigBnk| String | 非空 | 是否在18大行
crdTyp| String | 非空 | 卡种<br/>00:借记卡；<br/>01：贷记卡；<br/>02：预付费卡；<br/>04：准贷记卡


#### 1.4响应码说明 ####

code | 描述
---|---
SES00001| 传递参数qryCardNo为空
SES00002| 传递参数qryCardNo不是纯数字
SES00003| 传入卡号未匹配到卡bin信息
SES00000| 成功

