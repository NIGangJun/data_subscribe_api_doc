### 错误代码信息

错误代码（errcode） | 错误代码类型 | 错误信息 (errmsg) | 备注
---|---|---|--- 
0 | string | 请求成功 | 
1001 | string | 无数据 | 
1002 | string | 请求失败 | 
1003 | string | 账号验证无效 | 
1004 | string | 访问频率过快 | 
1005 | string | 缺少必要参数 | 
1006 | string | 此URL不存在 |
1007 | string | 被禁止的IP | 暂不使用
1008 | string | 接口维护 | 暂不使用
1009 | string | 接口停用 | 暂不使用


## 一、中国进出口税则


### 1. 中国税则基本信息


* **请求URL**
    * /services/cn_inout_tariff/cn_goods_tariff


* **请求类型**
    * GET


* **请求参数**

参数名称 | 参数类型 | 是否必填 | 备注
---|---|---|---
auth_key | string | 是 | 用户验证key
hs_code| string | 是 | 商品编码
page | int | 否 | 页码，默认为1


* **请求示例**
    * http://open_api.aeotrade.com/services/cn_inout_tariff/cn_goods_tariff?auth_key=1111111111&hs_code=1111111111&page=1


* **返回参数类型**
    * JSON


* **返回参数**

参数名称 | 参数类型 | 备注
---|---|---
errcode | string | 错误代码
errmsg | string | 错误信息
result | dict | 返回结果
&nbsp;&nbsp;&nbsp;&nbsp;page | int | 页码
&nbsp;&nbsp;&nbsp;&nbsp;total | int | 返回数据总数
&nbsp;&nbsp;&nbsp;&nbsp;data | list | 返回数据
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;hs_code | string | 商品编码
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;goods_name_cn | string | 商品中文名称
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;goods_name_en | string | 商品英文名称
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;goods_desc | string | 商品描述
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;unit_1_code | string | 第一计量单位代码
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;unit_1_name | string | 第一计量单位名称
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;unit_2_code | string | 第二计量单位代码
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;unit_2_name | string | 第二计量单位名称
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;goods_model_case | string | 申报要素填报案例
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;cus_control_code | string | 海关监管条件
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;ciq_control_code | string | 商检监管条件
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;im_ciq_special_doc_code | string | 进口报检特殊单证
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;im_ciq_note | string | 进口报检备注
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;ex_note | string | 出口备注

* **返回参数示例**


### 2. 进口基本税率


* **请求URL**
    * /services/cn_inout_tariff/im_base_rate


* **请求类型**
    * GET


* **请求参数**

参数名称 | 参数类型 | 是否必填 | 备注
---|---|---|---
auth_key | string | 是 | 用户验证key
hs_code| string | 是 | 商品编码
page | int | 否 | 页码，默认为1


* **请求示例**
    * http://open_api.aeotrade.com/services/cn_inout_tariff/im_base_rate?auth_key=1111111111&hs_code=1111111111&page=1


* **返回参数类型**
    * JSON


* **返回参数**

参数名称 | 参数类型 | 备注
---|---|---
errcode | string | 错误代码
errmsg | string | 错误信息
result | dict | 返回结果
&nbsp;&nbsp;&nbsp;&nbsp;page | int | 页码
&nbsp;&nbsp;&nbsp;&nbsp;total | int | 返回数据总数
&nbsp;&nbsp;&nbsp;&nbsp;data | list | 返回数据
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;hs_code | string | 商品编码
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;tax_category_name | string | 税种名称
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;tax_category_code | string | 税种编码
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;tax_type_code | string | 税率类别
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;rate_desc | string | 税率描述
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;rate_value | string | 税率值
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;specific_currency_code | string | 从量税币制
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;specific_unit_code | string | 从量税单位


* **返回参数示例**


### 3. 出口基本税率

* **请求URL**
    * /services/cn_inout_tariff/ex_base_rate


* **请求类型**
    * GET


* **请求参数**

参数名称 | 参数类型 | 是否必填 | 备注
---|---|---|---
auth_key | string | 是 | 用户验证key
hs_code| string | 是 | 商品编码
page | int | 否 | 页码，默认为1

* **请求示例**
    * http://open_api.aeotrade.com/services/cn_inout_tariff/ex_base_rate?auth_key=1111111111&hs_code=1111111111&page=1


* **返回参数类型**
    * JSON


* **返回参数**

参数名称 | 参数类型 | 备注
---|---|---
errcode | string | 错误代码
errmsg | string | 错误信息
result | dict | 返回结果
&nbsp;&nbsp;&nbsp;&nbsp;page | int | 页码
&nbsp;&nbsp;&nbsp;&nbsp;total | int | 返回数据总数
&nbsp;&nbsp;&nbsp;&nbsp;data | list | 返回数据
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;hs_code | string | 商品编码
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;tax_category_name | string | 税种名称
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;tax_category_code | string | 税种编码
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;tax_type_code | string | 税率类别
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;rate_desc | string | 税率描述
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;rate_value | string | 税率值
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;specific_currency_code | string | 从量税币制
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;specific_unit_code | string | 从量税单位


* **返回参数示例**


### 4. 进口特惠税率

* **请求URL**
    * /services/cn_inout_tariff/im_preferential_rate


* **请求类型**
    * GET


* **请求参数**

参数名称 | 参数类型 | 是否必填 | 备注
---|---|---|---
auth_key | string | 是 | 用户验证key
hs_code| string | 是 | 商品编码
page | int | 否 | 页码，默认为1


* **请求示例**
    * http://open_api.aeotrade.com/services/cn_inout_tariff/im_preferential_rate?auth_key=1111111111&hs_code=1111111111&page=1


* **返回参数类型**
    JSON


* **返回参数**

参数名称 | 参数类型 | 备注
---|---|---
errcode | string | 错误代码
errmsg | string | 错误信息
result | dict | 返回结果
&nbsp;&nbsp;&nbsp;&nbsp;page | int | 页码
&nbsp;&nbsp;&nbsp;&nbsp;total | int | 返回数据总数
&nbsp;&nbsp;&nbsp;&nbsp;data | list | 返回数据
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;hs_code | string | 商品编码
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;origin_country_code | string | 原产国代码
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;origin_country_name | string | 原产国名称
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;tax_category_name | string | 税种名称
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;tax_category_code | string | 税种编码
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;tax_type_code | string | 税率类别
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;rate_desc | string | 税率描述
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;rate_value | string | 税率值
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;specific_currency_code | string | 从量税币制
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;specific_unit_code | string | 从量税单位


* **返回参数示例**


### 5. 进口协定税率

* **请求URL**
    * /services/cn_inout_tariff/im_conventional_rate

* **请求类型**
    * GET


* **请求参数**

参数名称 | 参数类型 | 是否必填 | 备注
---|---|---|---
auth_key | string | 是 | 用户验证key
hs_code| string | 是 | 商品编码
page | int | 否 | 页码，默认为1


* **请求示例**
    * http://open_api.aeotrade.com/services/cn_inout_tariff/im_conventional_rate?auth_key=1111111111&hs_code=1111111111&page=1


* **返回参数类型**
    * JSON


* **返回参数**

参数名称 | 参数类型 | 备注
---|---|---
errcode | string | 错误代码
errmsg | string | 错误信息
result | dict | 返回结果
&nbsp;&nbsp;&nbsp;&nbsp;page | int | 页码
&nbsp;&nbsp;&nbsp;&nbsp;total | int | 返回数据总数
&nbsp;&nbsp;&nbsp;&nbsp;data | list | 返回数据
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;hs_code | string | 商品编码
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;origin_country_code | string | 原产国代码
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;origin_country_name | string | 原产国名称
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;tax_category_name | string | 税种名称
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;tax_category_code | string | 税种编码
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;tax_type_code | string | 税率类别
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;rate_desc | string | 税率描述
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;rate_value | string | 税率值
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;specific_currency_code | string | 从量税币制
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;specific_unit_code | string | 从量税单位


* **返回参数示例**


### 6. 进口双反税率
* **请求URL**
* **请求类型**
* **请求参数**
* **请求示例**
* **返回参数类型**
* **返回参数**
* **返回参数示例**


### 7. 废电基金征收标准
* **请求URL**
* **请求类型**
* **请求参数**
* **请求示例**
* **返回参数类型**
* **返回参数**
* **返回参数示例**


### 8. 申报要素
* **请求URL**
* **请求类型**
* **请求参数**
* **请求示例**
* **返回参数类型**
* **返回参数**
* **返回参数示例**


### 9. 检验检疫代码
* **请求URL**
* **请求类型**
* **请求参数**
* **请求示例**
* **返回参数类型**
* **返回参数**
* **返回参数示例**


### 10. 商品类目注释
* **请求URL**
* **请求类型**
* **请求参数**
* **请求示例**
* **返回参数类型**
* **返回参数**
* **返回参数示例**


## 二、归类参考


### 1. 中国出口申报实例
* **请求URL**
  * /services/classify_reference/cn_declare_element_eg


* **请求类型**
  * GET


* **请求参数**

| 参数名称 | 参数类型 | 是否必填 | 备注        |
| -------- | -------- | -------- | ----------- |
| auth_key | string   | 是       | 用户验证key |
| hs_code  | string   | 是       | 商品编码    |


* **请求示例**
  * http://open_api.aeotrade.com/services/classify_reference/cn_declare_element_eg?auth_key=1111111111&hs_code=1111111111


* **返回参数类型**
  * JSON

**返回参数**

| 参数名称                                                     | 参数类型 | 备注         |
| ------------------------------------------------------------ | -------- | ------------ |
| errcode                                                      | integer  | 错误代码     |
| errmsg                                                       | string   | 错误信息     |
| result                                                       | dict     | 返回结果     |
| &nbsp;&nbsp;&nbsp;&nbsp;page                                 | int      | 页码         |
| &nbsp;&nbsp;&nbsp;&nbsp;total                                | int      | 返回数据总数 |
| &nbsp;&nbsp;&nbsp;&nbsp;data                                 | list     | 返回数据     |
| &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;hs_code      | string   | 商品编码     |
| &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;goods_name_cn | string   | 商品中文名称 |
| &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;example_note | string   | 申报要素     |


### 2. 归类裁定
* **请求URL**

  * services/classify_reference/classify_ruling

* **请求类型**

  * GET

* **请求参数**

  * | 参数名称      | 参数类型 | 是否必填 | 备注         |
    | ------------- | -------- | -------- | ------------ |
    | auth_key      | string   | 是       | 用户验证key  |
    | related_no    | string   | 否       | 相关编号     |
    | goods_name_cn | string   | 否       | 商品中文名称 |

* **请求示例**

  * http://open_api.aeotrade.com/services/classify_reference/cn_declare_element_eg?auth_key=1111111111&related_no=1111111111&goods_name_cn=1111111111

* **返回参数类型**

  * JSON

* **返回参数**

  * | 参数名称                                                     | 参数类型 | 备注         |
    | ------------------------------------------------------------ | -------- | ------------ |
    | errcode                                                      | integer  | 错误代码     |
    | errmsg                                                       | string   | 错误信息     |
    | result                                                       | dict     | 返回结果     |
    | &nbsp;&nbsp;&nbsp;&nbsp;page                                 | int      | 页码         |
    | &nbsp;&nbsp;&nbsp;&nbsp;total                                | int      | 返回数据总数 |
    | &nbsp;&nbsp;&nbsp;&nbsp;data                                 | list     | 返回数据     |
    | &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;related_no   | string   | 相关编号     |
    | &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;resolve_duty_para | string   | 决定税号     |
    | &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;goods_name_cn | string   | 商品中文名称 |
    | &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;goods_name_en | string   | 商品英文名称 |
    | &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;goods_name_other | string   | 商品名称其他 |
    | &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;goods_desc   | string   | 商品描述     |
    | &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;classify_opinion                                             | string   | 归类意见     |
    | &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;issued_by                                                    | string   | 发布单位     |

* **返回参数示例**


### 3. 归类决定
* **请求URL**

  * /services/classify_reference/classify_resolve

* **请求类型**

  * GET

* **请求参数**

  * | 参数名称            | 参数类型 | 是否必填 | 备注         |
    | ------------------- | -------- | -------- | ------------ |
    | auth_key            | string   | 是       | 用户验证key  |
    | classify_resolve_no | string   | 否       | 归类决定编号 |
    | hs_code             | string   | 否       | 商品编码     |
    | goods_name_cn       | string   | 否       | 商品中文名称 |

* **请求示例**

  * http://open_api.aeotrade.com/services/classify_reference/cn_declare_element_eg?auth_key=1111111111&classify_resolve_no=1111111111&hs_code=1111111111&goods_name_cn=1111111111

* **返回参数类型**

  * JSON

* **返回参数**

  | 参数名称                                                     | 参数类型 | 备注         |
  | ------------------------------------------------------------ | -------- | ------------ |
  | errcode                                                      | integer  | 错误代码     |
  | errmsg                                                       | string   | 错误信息     |
  | result                                                       | dict     | 返回结果     |
  | &nbsp;&nbsp;&nbsp;&nbsp;page                                 | int      | 页码         |
  | &nbsp;&nbsp;&nbsp;&nbsp;total                                | int      | 返回数据总数 |
  | &nbsp;&nbsp;&nbsp;&nbsp;data                                 | list     | 返回数据     |
  | &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;classify_resolve_no | string   | 归类决定编号 |
  | &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;hs_code      | string   | 商品编码     |
  | &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;goods_name_cn | string   | 商品中文名称 |
  | &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;goods_name_en | string   | 商品英文名称 |
  | &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;goods_name_other | string   | 商品名称其他 |
  | &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;goods_desc   | string   | 商品描述     |
  | &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;classify_resolve_desc                                        | string   | 归类决定     |
  | &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;issued_by                                                    | string   | 发布单位     |

* **返回参数示例**


### 4. 归类预裁定
* **请求URL**

  * services/classify_reference/classify_pre_ruling

* **请求类型**

  * GET

* **请求参数**

  * * | 参数名称      | 参数类型 | 是否必填 | 备注             |
      | ------------- | -------- | -------- | ---------------- |
      | auth_key      | string   | 是       | 用户验证key      |
      | pre_ruling_no | string   | 否       | 预裁定决定书编号 |
      | hs_code       | string   | 否       | 商品编码         |
      | goods_name_cn | string   | 否       | 商品中文名称     |

* **请求示例**

  * http://open_api.aeotrade.com/services/classify_reference/cn_declare_element_eg?auth_key=1111111111&pre_ruling_no=11&hs_code=11&goods_name_cn=11

* **返回参数类型**

  * JSON

* **返回参数**

  * | 参数名称                                                     | 参数类型 | 备注                |
    | ------------------------------------------------------------ | -------- | ------------------- |
    | errcode                                                      | integer  | 错误代码            |
    | errmsg                                                       | string   | 错误信息            |
    | result                                                       | dict     | 返回结果            |
    | &nbsp;&nbsp;&nbsp;&nbsp;page                                 | int      | 页码                |
    | &nbsp;&nbsp;&nbsp;&nbsp;total                                | int      | 返回数据总数        |
    | &nbsp;&nbsp;&nbsp;&nbsp;data                                 | list     | 返回数据            |
    | &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;pre_ruling_no | string   | 预裁定决定书编号    |
    | &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;application_no | string   | 申请表编码          |
    | &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;hs_code      | string   | 商品编码            |
    | &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;goods_name_en | string   | 商品英文名称        |
    | &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;goods_name_other | string   | 商品名称其他        |
    | &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;goods_price_quantity_weight | string   | 商品价格、数量/重量 |
    | &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;goods_desc   | string   | 商品详细描述        |
    | &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;classify_pre_ruling_opinion                                  | string   | 商品归类预裁定意见  |

* **返回参数示例**


## 三、通关参数


### 1. 包装种类
* **请求URL**
* **请求类型**
* **请求参数**
* **请求示例**
* **返回参数类型**
* **返回参数**
* **返回参数示例**


### 2. 报关单类型
* **请求URL**

  * /services/cus_params/bill_entry_type

* **请求类型**

  * GET

* **请求参数**

  * | 参数名称 | 参数类型 | 是否必填 | 备注        |
    | -------- | -------- | -------- | ----------- |
    | auth_key | string   | 是       | 用户验证key |
    | keyword  | string   | 否       | 请求关键字  |
    | page     | int      | 否       | 页码        |

* **请求示例**

  * 示例1：http://open_api.aeotrade.com/services/cus_params/bill_entry_type?auth_key=123456789&keyword=M
  * 示例2：http://open_api.aeotrade.com/services/cus_params/bill_entry_type?auth_key=123456789&keyword=报关

* **返回参数类型**

  * JSON

* **返回参数**

  * | 参数名称 | 参数类型 | 备注               |
    | -------- | -------- | ------------------ |
    | errcode  | string   | 错误代码           |
    | errmsg   | string   | 错误信息           |
    | result   | dict     | 返回结果           |
    | page     | int      | 页码               |
    | total    | int      | 返回数据总数       |
    | data     | list     | 返回数据           |
    | code     | string   | 报关单类型代码     |
    | name_cn  | string   | 报关单类型中文名称 |

* **返回参数示例**

  * 示例1返回参数示例：

  * ```json
    {
        "errcode":"0",
        "errmsg":"请求成功",
        "result":{
            "page":1,
            "total":5,
            "data":[
                {
                    "code":"M",
                    "name_cn":"通关无纸化"
                }
    		]
        }
    }
    ```

  * 示例2返回参数示例：

  * ```json
    {
        "errcode":"0",
        "errmsg":"请求成功",
        "result":{
            "page":1,
            "total":5,
            "data":[
                {
                    "code":"O",
                    "name_cn":"有纸报关"
                },
                {
                    "code":"D",
                    "name_cn":"无纸带清单报关"
                },
                ......
        	]
        }
    }
    ```


### 3. 报关单单据类型
* **请求URL**

  * /services/cus_params/bill_entry_doc_type

* **请求类型**

  * GET

* **请求参数**

  * | 参数名称 | 参数类型 | 是否必填 | 备注        |
    | -------- | -------- | -------- | ----------- |
    | auth_key | string   | 是       | 用户验证key |
    | keyword  | string   | 否       | 请求关键字  |
    | page     | int      | 否       | 页码        |

* **请求示例**

  * 示例1：http://open_api.aeotrade.com/services/cus_params/bill_entry_doc_type?auth_key=123456789&keyword=C
  * 示例2：http://open_api.aeotrade.com/services/cus_params/bill_entry_doc_type?auth_key=123456789&keyword=自报自缴

* **返回参数类型**

  * JSON

* **返回参数**

  * | 参数名称 | 参数类型 | 备注                   |
    | -------- | -------- | ---------------------- |
    | errcode  | string   | 错误代码               |
    | errmsg   | string   | 错误信息               |
    | result   | dict     | 返回结果               |
    | page     | int      | 页码                   |
    | total    | int      | 返回数据总数           |
    | data     | list     | 返回数据               |
    | code     | string   | 报关单单据类型代码     |
    | name_cn  | string   | 报关单单据类型中文名称 |

* **返回参数示例**

  * 示例1返回参数示例：

  * ```json
    {
        "errcode":"0",
        "errmsg":"请求成功",
        "result":{
            "page":1,
            "total":18,
            "data":[
                {
                    "code":"CL",
                    "name_cn":"汇总征税报关单"
                },
                {
                    "code":"ZC",
                    "name_cn":"自报自缴，汇总征税报关单"
                },
                ......
    		]
        }
    }
    ```

  * 示例2返回参数示例：

  * ```json
    {
        "errcode":"0",
        "errmsg":"请求成功",
        "result":{
            "page":1,
            "total":18,
            "data":[
                {
                    "code":"Z",
                    "name_cn":"自报自缴"
                },
                {
                    "code":"ZC",
                    "name_cn":"自报自缴，汇总征税报关单"
                },
                ......
        	]
        }
    }
    ```


### 4. 备案清单类型
* **请求URL**

  * /services/cus_params/filing_doc_type

* **请求类型**

  * GET

* **请求参数**

  * | 参数名称 | 参数类型 | 是否必填 | 备注        |
    | -------- | -------- | -------- | ----------- |
    | auth_key | string   | 是       | 用户验证key |
    | keyword  | string   | 否       | 请求关键字  |
    | page     | int      | 否       | 页码        |

* **请求示例**

  * 示例1：http://open_api.aeotrade.com/services/cus_params/filing_doc_type?auth_key=123456789&keyword=1
  * 示例2：http://open_api.aeotrade.com/services/cus_params/filing_doc_type?auth_key=123456789&keyword=后报关

* **返回参数类型**

  * JSON

* **返回参数**

  * | 参数名称 | 参数类型 | 备注                 |
    | -------- | -------- | -------------------- |
    | errcode  | string   | 错误代码             |
    | errmsg   | string   | 错误信息             |
    | result   | dict     | 返回结果             |
    | page     | int      | 页码                 |
    | total    | int      | 返回数据总数         |
    | data     | list     | 返回数据             |
    | code     | string   | 备案清单类型代码     |
    | name_cn  | string   | 备案清单类型中文名称 |

* **返回参数示例**

  * 示例1返回参数示例：

  * ```json
    {
        "errcode":"0",
        "errmsg":"请求成功",
        "result":{
            "page":1,
            "total":4,
            "data":[
                {
                    "code":"1",
                    "name_cn":"一般备案清单"
                }
    		]
        }
    }
    ```

  * 示例2返回参数示例：

  * ```json
    {
        "errcode":"0",
        "errmsg":"请求成功",
        "result":{
            "page":1,
            "total":4,
            "data":[
                {
                    "code":"2",
                    "name_cn":"先进区、后报关"
                }
        	]
        }
    }
    ```


### 5. 成交方式
* **请求URL**
* **请求类型**
* **请求参数**
* **请求示例**
* **返回参数类型**
* **返回参数**
* **返回参数示例**


### 6. 港口代码
* **请求URL**
* **请求类型**
* **请求参数**
* **请求示例**
* **返回参数类型**
* **返回参数**
* **返回参数示例**


### 7. 关联理由代码
* **请求URL**
* **请求类型**
* **请求参数**
* **请求示例**
* **返回参数类型**
* **返回参数**
* **返回参数示例**


### 8. 关区代码
* **请求URL**

  * /services/cus_params/cus_dist_code

* **请求类型**

  * GET

* **请求参数**

  * | 参数名称 | 参数类型 | 是否必填 | 备注        |
    | -------- | -------- | -------- | ----------- |
    | auth_key | string   | 是       | 用户验证key |
    | keyword  | string   | 否       | 请求关键字  |
    | page     | int      | 否       | 页码        |

* **请求示例**

  * 示例1：http://open_api.aeotrade.com/services/cus_params/cus_dist_code?auth_key=123456789&keyword=010
  * 示例2：http://open_api.aeotrade.com/services/cus_params/cus_dist_code?auth_key=123456789&keyword=海关总署

* **返回参数类型**

  * JSON

* **返回参数**

  * | 参数名称 | 参数类型 | 备注         |
    | -------- | -------- | ------------ |
    | errcode  | string   | 错误代码     |
    | errmsg   | string   | 错误信息     |
    | result   | dict     | 返回结果     |
    | page     | int      | 页码         |
| total    | int      | 返回数据总数 |
| data     | list     | 返回数据     |
    | code     | string   | 关区代码     |
    | name_cn  | string   | 关区中文名称 |

* **返回参数示例**

  * 示例1返回参数：

  * ```json
    {
        "errcode":"0",
        "errmsg":"请求成功",
        "result":{
            "page":1,
            "total":1325,
            "data":[
                {
                    "code":"0100",
                    "name_cn":"北京关区"
                },
                 {
                    "code":"0101",
                    "name_cn":"京机场关"
                },
                ......
    	]
        }
  }
    ```
    
  * 示例2返回参数：
  
  * ```json
    {
        "errcode":"0",
        "errmsg":"请求成功",
        "result":{
            "page":1,
            "total":1325,
            "data":[
                {
                    "code":"0000",
                    "name_cn":"海关总署"
                }
        	]
        }
    }
    ```


### 9. 国别地区代码
* **请求URL**

  * /services/cus_params/foreign_region_code

* **请求类型**

  * GET

* **请求参数**

  * | 参数名称 | 参数类型 | 是否必填 | 备注        |
    | -------- | -------- | -------- | ----------- |
    | auth_key | string   | 是       | 用户验证key |
    | keyword  | string   | 否       | 请求关键字  |
    | page     | int      | 否       | 页码        |

* **请求示例**

  * 示例1：http://open_api.aeotrade.com/services/cus_params/foreign_region_code?auth_key=123456789&keyword=ABW
  * 示例2：http://open_api.aeotrade.com/services/cus_params/foreign_region_code?auth_key=123456789&keyword=阿富汗

* **返回参数类型**

  * JSON

* **返回参数**

  * | 参数名称     | 参数类型 | 备注         |
    | ------------ | -------- | ------------ |
    | errcode      | string   | 错误代码     |
    | errmsg       | string   | 错误信息     |
    | result       | dict     | 返回结果     |
    | page         | int      | 页码         |
    | total        | int      | 返回数据总数 |
    | data         | list     | 返回数据     |
    | code         | string   | 国别代码     |
    | name_cn      | string   | 国别中文名称 |
    | dec_old_code | string   | 原海关代码   |
    | ciq_old_code | string   | 原检疫代码   |

* **返回参数示例**

  * 示例1返回参数：

  * ```json
    {
        "errcode":"0",
        "errmsg":"请求成功",
        "result":{
            "page":1,
            "total":265,
            "data":[
                {
                    "code":"ABW",
                	"name_cn":"阿鲁巴",
                	"dec_old_code":"403",
                	"ciq_old_code":"533"
                }
    	]
        }
  }
    
    ```
    
  * 示例2返回参数：
  
  * ```json
    {
        "errcode":"0",
        "errmsg":"请求成功",
        "result":{
            "page":1,
            "total":265,
            "data":[
                {
                    "code":"AFG",
                	"name_cn":"阿富汗",
                	"dec_old_code":"101",
                	"ciq_old_code":"004"
            	}
        	]
        }
    }
    ```


### 10. 国内地区代码
* **请求URL**

  * /services/cus_params/inland_region_code

* **请求类型**

  * GET

* **请求参数**

  * | 参数名称 | 参数类型 | 是否必填 | 备注        |
    | -------- | -------- | -------- | ----------- |
    | auth_key | string   | 是       | 用户验证key |
    | keyword  | string   | 否       | 请求关键字  |
    | page     | int      | 否       | 页码        |

* **请求示例**

  * 示例1：http://open_api.aeotrade.com/services/cus_params/inland_region_code?auth_key=123456789&keyword=640
  * 示例2：http://open_api.aeotrade.com/services/cus_params/inland_region_code?auth_key=123456789&keyword=石嘴山

* **返回参数类型**

  * JSON

* **返回参数**

  * | 参数名称 | 参数类型 | 备注             |
    | -------- | -------- | ---------------- |
    | errcode  | string   | 错误代码         |
    | errmsg   | string   | 错误信息         |
    | result       | dict     | 返回结果     |
    | page         | int      | 页码         |
    | total        | int      | 返回数据总数 |
    | data         | list     | 返回数据     |
    | code     | string   | 国内地区代码     |
    | name_cn  | string   | 国内地区中文名称 |

* **返回参数示例**

  * 示例1返回参数：

  * ```json
    {
        "errcode":"0",
        "errmsg":"请求成功",
        "result":{
            "page":1,
            "total":1048,
            "data":[
               	{
                	"code":"64019",
                	"name_cn":"银川"
            	},
                {
                    "code":"64029",
                    "name_cn":"石嘴山"
                },
                ......
    	]
        }
  }
    ```
    
  * 示例2返回参数：
  
  * ```json
    {
        "errcode":"0",
        "errmsg":"请求成功",
        "result":{
            "page":1,
            "total":1048,
            "data":[
               {
                    "code":"64029",
                    "name_cn":"石嘴山"
                },
                {
                    "code":"6402W",
                    "name_cn":"石嘴山保税物流中心（B型）"
                },
                ......
        	]
        }
    }
    ```


### 11. 国内口岸代码
* **请求URL**
* **请求类型**
* **请求参数**
* **请求示例**
* **返回参数类型**
* **返回参数**
* **返回参数示例**


### 12. 货币代码
* **请求URL**

  * /services/cus_params/currency_code

* **请求类型**

  * GET

* **请求参数**

  * | 参数名称 | 参数类型 | 是否必填 | 备注        |
    | -------- | -------- | -------- | ----------- |
    | auth_key | string   | 是       | 用户验证key |
    | keyword  | string   | 否       | 请求关键字  |
    | page     | int      | 否       | 页码        |

* **请求示例**

  * 示例1：http://open_api.aeotrade.com/services/cus_params/currency_code?auth_key=123456789&keyword=AUD
  * 示例2：http://open_api.aeotrade.com/services/cus_params/currency_code?auth_key=123456789&keyword=人民币
  
* **返回参数类型**

  * JSON

* **返回参数**

  * | 参数名称     | 参数类型 | 备注         |
    | ------------ | -------- | ------------ |
    | errcode      | string   | 错误代码     |
    | errmsg       | string   | 错误信息     |
    | result       | dict     | 返回结果     |
    | page         | int      | 页码         |
    | total        | int      | 返回数据总数 |
    | data         | list     | 返回数据     |
    | code         | string   | 货币代码     |
    | symbol       | string   | 货币符号     |
    | name_cn      | string   | 货币中文名称 |
    | dec_old_code | string   | 原海关代码   |
    | ciq_old_code | string   | 原检疫代码   |

* **返回参数示例**

  * 示例1返回参数：

  * ```json
    {
        "errcode":"0",
        "errmsg":"请求成功",
        "result":{
            "page":1,
            "total":22,
            "data":[
               {
                    "code":"AUD",
                    "symbol":"$",
                    "name_cn":"澳大利亚元",
                    "dec_old_code":"601",
                    "ciq_old_code":"36"
                }
    	]
        }
  }
    ```
    
  * 示例2返回参数：
  
  * ```json
    {
        "errcode":"0",
        "errmsg":"请求成功",
        "result":{
            "page":1,
            "total":22,
            "data":[
                 {
                    "code":"CNY",
                    "symbol":"¥",
                  	"name_cn":"人民币",
                    "dec_old_code":"142",
                  	"ciq_old_code":"156"
                 }
      	]
        }
    }
    ```
    


### 13. 货物属性
* **请求URL**

  * /services/cus_params/goods_attr_type

* **请求类型**

  * GET

* **请求参数**

  * | 参数名称 | 参数类型 | 是否必填 | 备注        |
    | -------- | -------- | -------- | ----------- |
    | auth_key | string   | 是       | 用户验证key |
    | keyword  | string   | 否       | 请求关键字  |
    | page     | int      | 否       | 页码        |

* **请求示例**

  * 示例1：http://open_api.aeotrade.com/services/cus_params/goods_attr_type?auth_key=123456789&keyword=12
  * 示例2：http://open_api.aeotrade.com/services/cus_params/goods_attr_type?auth_key=123456789&keyword=转基因产品

* **返回参数类型**

  * JSON

* **返回参数**

  * | 参数名称 | 参数类型 | 备注             |
    | -------- | -------- | ---------------- |
    | errcode  | string   | 错误代码         |
    | errmsg   | string   | 错误信息         |
    | result   | dict     | 返回结果         |
    | page     | int      | 页码             |
    | total    | int      | 返回数据总数     |
    | data     | list     | 返回数据         |
    | code     | string   | 货物属性代码     |
    | name_cn  | string   | 货物属性中文名称 |

* **返回参数示例**

  * 示例1返回参数示例：

  * ```json
    {
        "errcode":"0",
        "errmsg":"请求成功",
        "result":{
            "page":1,
            "total":20,
            "data":[
                {
                    "code":"12",
                    "name_cn":"3C目录外"
                }
    		]
        }
    }
    ```

  * 示例2返回参数示例：

  * ```json
    {
        "errcode":"0",
        "errmsg":"请求成功",
        "result":{
            "page":1,
            "total":4,
            "data":[
                {
                    "code":"16",
                    "name_cn":"转基因产品"
                }
        	]
        }
    }
    ```


### 14. 货物用途
* **请求URL**

  * /services/cus_params/goods_purpose

* **请求类型**

  * GET

* **请求参数**

  * | 参数名称 | 参数类型 | 是否必填 | 备注        |
    | -------- | -------- | -------- | ----------- |
    | auth_key | string   | 是       | 用户验证key |
    | keyword  | string   | 否       | 请求关键字  |
    | page     | int      | 否       | 页码        |

* **请求示例**

  * 示例1：http://open_api.aeotrade.com/services/cus_params/goods_purpose?auth_key=123456789&keyword=12
  * 示例2：http://open_api.aeotrade.com/services/cus_params/goods_purpose?auth_key=123456789&keyword=化妆品

* **返回参数类型**

  * JSON

* **返回参数**

  * | 参数名称 | 参数类型 | 备注             |
    | -------- | -------- | ---------------- |
    | errcode  | string   | 错误代码         |
    | errmsg   | string   | 错误信息         |
    | result   | dict     | 返回结果         |
    | page     | int      | 页码             |
    | total    | int      | 返回数据总数     |
    | data     | list     | 返回数据         |
    | code     | string   | 货物用途代码     |
    | name_cn  | string   | 货物用途中文名称 |

* **返回参数示例**

  * 示例1返回参数示例：

  * ```json
    {
        "errcode":"0",
        "errmsg":"请求成功",
        "result":{
            "page":1,
            "total":20,
            "data":[
                {
                    "code":"12",
                    "name_cn":"食用"
                }
    		]
        }
    }
    ```

  * 示例2返回参数示例：

  * ```json
    {
        "errcode":"0",
        "errmsg":"请求成功",
        "result":{
            "page":1,
            "total":4,
            "data":[
                {
                    "code":"27",
                    "name_cn":"化妆品"
                },
                {
                    "code":"28",
                    "name_cn":"化妆品原料"
                }
        	]
        }
    }
    ```


### 15. 集装箱规格
* **请求URL**

  * /services/cus_params/container_spec

* **请求类型**

  * GET

* **请求参数**

  * | 参数名称 | 参数类型 | 是否必填 | 备注        |
    | -------- | -------- | -------- | ----------- |
    | auth_key | string   | 是       | 用户验证key |
    | keyword  | string   | 否       | 请求关键字  |
    | page     | int      | 否       | 页码        |

* **请求示例**

  * 示例1：http://open_api.aeotrade.com/services/cus_params/container_spec?auth_key=123456789&keyword=11
  * 示例2：http://open_api.aeotrade.com/services/cus_params/container_spec?auth_key=123456789&keyword=标准

* **返回参数类型**

  * JSON

* **返回参数**

  * | 参数名称     | 参数类型 | 备注               |
    | ------------ | -------- | ------------------ |
    | errcode      | string   | 错误代码           |
    | errmsg       | string   | 错误信息           |
    | result       | dict     | 返回结果           |
    | page         | int      | 页码               |
    | total        | int      | 返回数据总数       |
    | data         | list     | 返回数据           |
    | code         | string   | 集装箱规格代码     |
    | name_cn      | string   | 集装箱规格中文名称 |
    | dec_old_code | string   | 原海关代码         |
    | ciq_old_code | string   | 原检疫代码         |

* **返回参数示例**

  * 示例1返回参数：

  * ```json
    {
        "errcode":"0",
        "errmsg":"请求成功",
        "result":{
            "page":1,
            "total":9,
            "data":[
                 {
                   "code":"11",
                    "name_cn":"普通2*标准箱（L）",
                    "dec_old_code":"L",
                    "ciq_old_code":"111"
                 }
    	]
        }
  }
    ```
    
  * 示例2返回参数：
  
  * ```json
    {
        "errcode":"0",
        "errmsg":"请求成功",
        "result":{
            "page":1,
            "total":9,
            "data":[
                 {
                    "code":"11",
                    "name_cn":"普通2*标准箱（L）",
                    "dec_old_code":"L",
                    "ciq_old_code":"111"
                },
                {
                    "code":"12",
                    "name_cn":"冷藏2*标准箱（L）",
                    "dec_old_code":"L",
                    "ciq_old_code":"121"
                },
                ......
        	]
        }
    }
    ```


### 16. 计量单位
* **请求URL**
* **请求类型**
* **请求参数**
* **请求示例**
* **返回参数类型**
* **返回参数**
* **返回参数示例**


### 17. 监管方式
* **请求URL**
* **请求类型**
* **请求参数**
* **请求示例**
* **返回参数类型**
* **返回参数**
* **返回参数示例**


### 18. 检验检疫机关代码
* **请求URL**

  * /services/cus_params/ciq_org_code

* **请求类型**

  * GET

* **请求参数**

  * | 参数名称 | 参数类型 | 是否必填 | 备注        |
    | -------- | -------- | -------- | ----------- |
    | auth_key | string   | 是       | 用户验证key |
    | keyword  | string   | 否       | 请求关键字  |
    | page     | int      | 否       | 页码        |

* **请求示例**

  * 示例1：http://open_api.aeotrade.com/services/cus_params/ciq_org_code?auth_key=123456789&keyword=000000
  * 示例2：http://open_api.aeotrade.com/services/cus_params/ciq_org_code?auth_key=123456789&keyword=海关

* **返回参数类型**

  * JSON

* **返回参数**

  * | 参数名称 | 参数类型 | 备注         |
    | -------- | -------- | ------------ |
    | errcode  | string   | 错误代码     |
    | errmsg   | string   | 错误信息     |
    | result       | dict     | 返回结果     |
    | page         | int      | 页码         |
    | total        | int      | 返回数据总数 |
    | data         | list     | 返回数据     |
    | code     | string   | 机关代码     |
    | name_cn  | string   | 机关中文名称 |

* **返回参数示例**

  * 示例1返回参数示例：

  * ```json
    {
        "errcode":"0",
        "errmsg":"请求成功",
        "result":{
            "page":1,
            "total":870,
            "data":[
                {
                    "code":"000000",
                    "name_cn":"海关总署"
                }
    	]
        }
  }
    ```
    
  * 示例2返回参数示例：
  
  * ```json
    {
        "errcode":"0",
        "errmsg":"请求成功",
        "result":{
            "page":1,
            "total":870,
            "data":[
                {
                    "code":"110000",
                    "name_cn":"北京海关本部"
                },
                {
                    "code":"115100",
                    "name_cn":"首都机场海关本部"
                },
                ......
        	]
        }
    }
    ```


### 19. 企业资质类别
* **请求URL**

  * /services/cus_params/ent_qua_type

* **请求类型**

  * GET

* **请求参数**

  * | 参数名称 | 参数类型 | 是否必填 | 备注        |
    | -------- | -------- | -------- | ----------- |
    | auth_key | string   | 是       | 用户验证key |
    | keyword  | string   | 否       | 请求关键字  |
    | page     | int      | 否       | 页码        |

* **请求示例**

  * 示例1：http://open_api.aeotrade.com/services/cus_params/ent_qua_type?auth_key=123456789&keyword=100
  * 示例2：http://open_api.aeotrade.com/services/cus_params/ent_qua_type?auth_key=123456789&keyword=进口肉类

* **返回参数类型**

  * JSON

* **返回参数**

  * | 参数名称 | 参数类型 | 备注             |
    | -------- | -------- | ---------------- |
    | errcode  | string   | 错误代码         |
    | errmsg   | string   | 错误信息         |
    | result   | dict     | 返回结果         |
    | page     | int      | 页码             |
    | total    | int      | 返回数据总数     |
    | data     | list     | 返回数据         |
    | code     | string   | 企业资质代码     |
    | name_cn  | string   | 企业资质中文名称 |

* **返回参数示例**

  * 示例1返回参数示例：

  * ```json
    {
        "errcode":"0",
        "errmsg":"请求成功",
        "result":{
            "page":1,
            "total":35,
            "data":[
                {
                    "code":"100",
                    "name_cn":"通关司类"
                }
    	]
        }
    }
    ```

  * 示例2返回参数示例：

  * ```json
    {
        "errcode":"0",
        "errmsg":"请求成功",
        "result":{
            "page":1,
            "total":35,
            "data":[
                {
                    "code":"510",
                    "name_cn":"进口肉类收货人备案"
                },
                {
                    "code":"511",
                    "name_cn":"进口肉类存储冷库备案"
                },
                ......
        	]
        }
    }
    ```


### 20. 检验检疫申请单证代码
* **请求URL**

  * /services/cus_params/ciq_app_doc_code

* **请求类型**

  * GET

* **请求参数**

  * | 参数名称 | 参数类型 | 是否必填 | 备注        |
    | -------- | -------- | -------- | ----------- |
    | auth_key | string   | 是       | 用户验证key |
    | keyword  | string   | 否       | 请求关键字  |
    | page     | int      | 否       | 页码        |

* **请求示例**

  * 示例1：http://open_api.aeotrade.com/services/cus_params/ciq_app_doc_code?auth_key=123456789&keyword=18
  * 示例2：http://open_api.aeotrade.com/services/cus_params/ciq_app_doc_code?auth_key=123456789&keyword=证书

* **返回参数类型**

  * JSON

* **返回参数**

  * | 参数名称 | 参数类型 | 备注             |
    | -------- | -------- | ---------------- |
    | errcode  | string   | 错误代码         |
    | errmsg   | string   | 错误信息         |
    | result       | dict     | 返回结果     |
    | page         | int      | 页码         |
    | total        | int      | 返回数据总数 |
    | data         | list     | 返回数据     |
    | code     | string   | 申请单证代码     |
    | name_cn  | string   | 申请单证中文名称 |

* **返回参数示例**

  * 示例1返回参数示例：

  * ```json
    {
        "errcode":"0",
        "errmsg":"请求成功",
        "result":{
            "page":1,
            "total":19,
            "data":[
                {
                    "code":"18",
                    "name_cn":"植物检疫证书"
                }
    	]
        }
  }
    ```
    
  * 示例2返回参数示例：
  
  * ```json
    {
        "errcode":"0",
        "errmsg":"请求成功",
        "result":{
            "page":1,
            "total":19,
            "data":[
               {
                    "code":"11",
                    "name_cn":"品质证书"
                },
                {
                    "code":"12",
                    "name_cn":"重量证书"
                },
                ......
        	]
        }
    }
    ```


### 21. 世界各国地区代码
* **请求URL**
* **请求类型**
* **请求参数**
* **请求示例**
* **返回参数类型**
* **返回参数**
* **返回参数示例**


### 22. 随附单证类型
* **请求URL**

  * /services/cus_params/doc_att_type

* **请求类型**

  * GET

* **请求参数**

  * | 参数名称 | 参数类型 | 是否必填 | 备注        |
    | -------- | -------- | -------- | ----------- |
    | auth_key | string   | 是       | 用户验证key |
    | keyword  | string   | 否       | 请求关键字  |
    | page     | int      | 否       | 页码        |

* **请求示例**

  * 示例1：http://open_api.aeotrade.com/services/cus_params/doc_att_type?auth_key=123456789&keyword=A
  * 示例2：http://open_api.aeotrade.com/services/cus_params/doc_att_type?auth_key=123456789&keyword=出口许可证

* **返回参数类型**

  * JSON

* **返回参数**

  * | 参数名称 | 参数类型 | 备注             |
    | -------- | -------- | ---------------- |
    | errcode  | string   | 错误代码         |
    | errmsg   | string   | 错误信息         |
    | result       | dict     | 返回结果     |
    | page         | int      | 页码         |
    | total        | int      | 返回数据总数 |
    | data         | list     | 返回数据     |
    | code     | string   | 随附单证类型代码 |
    | name_cn  | string   | 随附单证类型中文名称 |

* **返回参数示例**

  * 示例1返回参数示例：

  * ```json
    {
        "errcode":"0",
        "errmsg":"请求成功",
        "result":{
            "page":1,
            "total":55,
            "data":[
               {
                    "code":"A",
                    "name_cn":"检验检疫"
                }
    	]
        }
  }
    ```
    
  * 示例2返回参数示例：
  
  * ```json
    {
        "errcode":"0",
        "errmsg":"请求成功",
        "result":{
            "page":1,
            "total":55,
            "data":[
              	{
                    "code":"3",
                    "name_cn":"两用物项和技术出口许可证"
                },
                {
                    "code":"5",
                    "name_cn":"纺织品临时出口许可证"
                }
                ......
        	]
        }
    }
    ```


### 23. 随附单据类型
* **请求URL**

  * /services/cus_params/bill_att_type

* **请求类型**

  * GET

* **请求参数**

  * | 参数名称 | 参数类型 | 是否必填 | 备注        |
    | -------- | -------- | -------- | ----------- |
    | auth_key | string   | 是       | 用户验证key |
    | keyword  | string   | 否       | 请求关键字  |
    | page     | int      | 否       | 页码        |

* **请求示例**

  * 示例1：http://open_api.aeotrade.com/services/cus_params/bill_att_type?auth_key=123456789&keyword=010
  * 示例2：http://open_api.aeotrade.com/services/cus_params/bill_att_type?auth_key=123456789&keyword=检疫证书

* **返回参数类型**

  * JSON

* **返回参数**

  * | 参数名称 | 参数类型 | 备注             |
    | -------- | -------- | ---------------- |
    | errcode  | string   | 错误代码         |
    | errmsg   | string   | 错误信息         |
    | result       | dict     | 返回结果     |
    | page         | int      | 页码         |
    | total        | int      | 返回数据总数 |
    | data         | list     | 返回数据     |
    | code     | string   | 随附单据类型代码 |
    | name_cn  | string   | 随附单据类型中文名称 |

* **返回参数示例**

  * 示例1返回参数示例：

  * ```json
    {
        "errcode":"0",
        "errmsg":"请求成功",
        "result":{
            "page":1,
            "total":59,
            "data":[
              	{
                    "code":"00000010",
                    "name_cn":"载货清单（舱单）"
                },
                {
                    "code":"50000010",
                    "name_cn":"特殊医学用途配方食品注册证书"
                }
                ......
    	]
        }
  }
    ```
    
  * 示例2返回参数示例：
  
  * ```json
    {
        "errcode":"0",
        "errmsg":"请求成功",
        "result":{
            "page":1,
            "total":59,
            "data":[
              	{
                    "code":"20000012",
                    "name_cn":"动物检疫证书"
                },
                {
                    "code":"20000013",
                    "name_cn":"植物检疫证书"
                }
                ......
        	]
        }
    }
    ```


### 24. 危包类别
* **请求URL**

  * /services/cus_params/dang_pack_categ

* **请求类型**

  * GET

* **请求参数**

  * | 参数名称 | 参数类型 | 是否必填 | 备注        |
    | -------- | -------- | -------- | ----------- |
    | auth_key | string   | 是       | 用户验证key |
    | keyword  | string   | 否       | 请求关键字  |
    | page     | int      | 否       | 页码        |

* **请求示例**

  * 示例1：http://open_api.aeotrade.com/services/cus_params/dang_pack_spec?auth_key=123456789&keyword=3
  * 示例2：http://open_api.aeotrade.com/services/cus_params/dang_pack_spec?auth_key=123456789&keyword=二类

* **返回参数类型**

  * JSON

* **返回参数**

  * | 参数名称 | 参数类型 | 备注             |
    | -------- | -------- | ---------------- |
    | errcode  | string   | 错误代码         |
    | errmsg   | string   | 错误信息         |
    | result       | dict     | 返回结果     |
    | page         | int      | 页码         |
    | total        | int      | 返回数据总数 |
    | data         | list     | 返回数据     |
    | code     | string   | 危包类别代码     |
    | name_cn  | string   | 危包类别中文名称 |

* **返回参数示例**

  * 示例1返回参数示例：

  * ```json
    {
        "errcode":"0",
        "errmsg":"请求成功",
        "result":{
            "page":1,
            "total":3,
            "data":[
              	{
                    "code":"3",
                    "name_cn":"三类"
                }
    	]
        }
  }
    ```
    
  * 示例2返回参数示例：
  
  * ```json
    {
        "errcode":"0",
        "errmsg":"请求成功",
        "result":{
            "page":1,
            "total":3,
            "data":[
              	{
                    "code":"2",
                    "name_cn":"二类"
                }
        	]
        }
    }
    ```


### 25. 危包规格
* **请求URL**

  * /services/cus_params/dang_pack_spec

* **请求类型**

  * GET

* **请求参数**

  * | 参数名称 | 参数类型 | 是否必填 | 备注        |
    | -------- | -------- | -------- | ----------- |
    | auth_key | string   | 是       | 用户验证key |
    | keyword  | string   | 否       | 请求关键字  |
    | page     | int      | 否       | 页码        |

* **请求示例**

  * 示例：http://open_api.aeotrade.com/services/cus_params/dang_pack_spec?auth_key=123456789&keyword=4A
  
* **返回参数类型**

  * JSON

* **返回参数**

  * | 参数名称 | 参数类型 | 备注             |
    | -------- | -------- | ---------------- |
    | errcode  | string   | 错误代码         |
    | errmsg   | string   | 错误信息         |
    | result       | dict     | 返回结果     |
    | page         | int      | 页码         |
    | total        | int      | 返回数据总数 |
    | data         | list     | 返回数据     |
    | code     | string   | 危包规格代码     |
    | name_cn  | string   | 危包规格中文名称 |

* **返回参数示例**

  * 示例返回参数示例：

  * ```json
    {
        "errcode":"1001",
        "errmsg":"无数据",
        "result":{
            "page":1,
            "total":0,
            "data":[]
        }
}
    ```
  


### 26. 许可证类别代码
* **请求URL**
* **请求类型**
* **请求参数**
* **请求示例**
* **返回参数类型**
* **返回参数**
* **返回参数示例**


### 27. 运输方式
* **请求URL**
* **请求类型**
* **请求参数**
* **请求示例**
* **返回参数类型**
* **返回参数**
* **返回参数示例**


### 28. 征免方式
* **请求URL**

  * /services/cus_params/nat_levy_mode

* **请求类型**

  * GET

* **请求参数**

  * | 参数名称 | 参数类型 | 是否必填 | 备注        |
    | -------- | -------- | -------- | ----------- |
    | auth_key | string   | 是       | 用户验证key |
    | keyword  | string   | 否       | 请求关键字  |
    | page     | int      | 否       | 页码        |

* **请求示例**

  * 示例1：http://open_api.aeotrade.com/services/cus_params/nat_levy_exem?auth_key=123456789&keyword=5
  * 示例2：http://open_api.aeotrade.com/services/cus_params/nat_levy_exem?auth_key=123456789&keyword=征税

* **返回参数类型**

  * JSON

* **返回参数**

  * | 参数名称 | 参数类型 | 备注             |
    | -------- | -------- | ---------------- |
    | errcode  | string   | 错误代码         |
    | errmsg   | string   | 错误信息         |
    | result   | dict     | 返回结果         |
    | page     | int      | 页码             |
    | total    | int      | 返回数据总数     |
    | data     | list     | 返回数据         |
    | code     | string   | 征免方式代码     |
    | name_cn  | string   | 征免方式中文名称 |

* **返回参数示例**

  * 示例1返回参数示例：

  * ```json
    {
        "errcode":"0",
        "errmsg":"请求成功",
        "result":{
            "page":1,
            "total":8,
            "data":[
                {
                    "code":"5",
                    "name_cn":"征免性质"
                } 
            ]
        }
    }
    ```

  * 示例2返回参数示例：

  * ```json
    {
        "errcode":"0",
        "errmsg":"请求成功",
        "result":{
            "page":1,
            "total":8,
            "data":[
                {
                    "code":"1",
                    "name_cn":"照章征税"
                },
                {
                    "code":"2",
                    "name_cn":"折半征税"
                },
                ......
            ]
        }
    }
    ```


### 29. 征免性质
* **请求URL**

  * /services/cus_params/nat_levy_exem

* **请求类型**

  * GET

* **请求参数**

  * | 参数名称 | 参数类型 | 是否必填 | 备注        |
    | -------- | -------- | -------- | ----------- |
    | auth_key | string   | 是       | 用户验证key |
    | keyword  | string   | 否       | 请求关键字  |
    | page     | int      | 否       | 页码        |

* **请求示例**

  * 示例1：http://open_api.aeotrade.com/services/cus_params/nat_levy_exem?auth_key=123456789&keyword=101
  * 示例2：http://open_api.aeotrade.com/services/cus_params/nat_levy_exem?auth_key=123456789&keyword=征税

* **返回参数类型**

  * JSON

* **返回参数**

  * | 参数名称 | 参数类型 | 备注             |
    | -------- | -------- | ---------------- |
    | errcode  | string   | 错误代码         |
    | errmsg   | string   | 错误信息         |
    | result       | dict     | 返回结果     |
    | page         | int      | 页码         |
    | total        | int      | 返回数据总数 |
    | data         | list     | 返回数据     |
    | code     | string   | 征免性质代码     |
    | name_cn  | string   | 征免性质中文名称 |

* **返回参数示例**

  * 示例1返回参数示例：

  * ```json
    {
        "errcode":"0",
        "errmsg":"请求成功",
        "result":{
            "page":1,
            "total":78,
            "data":[
                {
                    "code":"101",
                    "name_cn":"一般征税"
                } 
        ]
        }
  }
    ```
    
  * 示例2返回参数示例：
  
  * ```json
    {
        "errcode":"0",
        "errmsg":"请求成功",
        "result":{
            "page":1,
            "total":78,
            "data":[
                {
                    "code":"101",
                    "name_cn":"一般征税"
                },
                {
                    "code":"118",
                    "name_cn":"整车征税"
                },
                ......
            ]
        }
    }
    ```


### 30. 中国行政区划
* **请求URL**

  * /services/cus_params/cn_admin_area

* **请求类型**

  * GET

* **请求参数**

  * | 参数名称 | 参数类型 | 是否必填 | 备注        |
    | -------- | -------- | -------- | ----------- |
    | auth_key | string   | 是       | 用户验证key |
    | keyword  | string   | 否       | 请求关键字  |
    | page     | int      | 否       | 页码        |

* **请求示例**

  * 示例1：http://open_api.aeotrade.com/services/cus_params/cn_admin_area?auth_key=123456789&keyword=654026
  * 示例2：http://open_api.aeotrade.com/services/cus_params/cn_admin_area?auth_key=123456789&keyword=中国

* **返回参数类型**

  * JSON

* **返回参数**

  * | 参数名称 | 参数类型 | 备注                 |
    | -------- | -------- | -------------------- |
    | errcode  | string   | 错误代码             |
    | errmsg   | string   | 错误信息             |
    | result   | dict     | 返回结果             |
    | page     | int      | 页码                 |
    | total    | int      | 返回数据总数         |
    | data     | list     | 返回数据             |
    | code     | string   | 国内行政区划代码     |
    | name_cn  | string   | 国内行政区划中文名称 |

* **返回参数示例**

  * 示例1返回参数示例：

  * ```json
    {
        "errcode":"0",
        "errmsg":"请求成功",
        "result":{
            "page":1,
            "total":3433,
            "data":[
                {
                    "code":"654026",
                    "name_cn":"伊犁哈萨克自治州昭苏县"
                } 
        	]
        }
    }
    ```

  * 示例2返回参数示例：

  * ```json
    {
        "errcode":"0",
        "errmsg":"请求成功",
        "result":{
            "page":1,
            "total":3433,
            "data":[
                {
                    "code":"910000",
                    "name_cn":"中国"
                }
            ]
        }
    }
    ```


### 


## 四、贸易管制商品目录
## 五、贸易单证数据
## 六、其他