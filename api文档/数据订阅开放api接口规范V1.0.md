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
hs_code| string | 否 | 商品编码
goods_name_cn | string | 否 | 商品中文名称
goods_name_en | string | 否 | 商品英文名称
page | int | 否 | 页码


* **请求示例**
    * http://open_api.aeotrade.com/services/cn_inout_tariff/cn_goods_tariff?auth_key=1111111111&hs_code=1111111111&goods_name_cn=口罩&goods_name_cn=apple


* **返回参数类型**
    * JSON


* **返回参数**

参数名称 | 参数类型 | 备注
---|---|---
errcode | integer | 错误代码
errmsg | string | 错误信息
result | dict | 返回结果
&nbsp;&nbsp;&nbsp;&nbsp;page | int | 页码
&nbsp;&nbsp;&nbsp;&nbsp;total | int | 返回数据总数
&nbsp;&nbsp;&nbsp;&nbsp;data | dict | 返回数据
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
    * /services/cn_inout_tariff/cn_im_base_rate
* **请求类型**
    * GET
* **请求参数**

参数名称 | 参数类型 | 是否必填 | 备注
---|---|---|---
auth_key | string | 是 | 用户验证key
hs_code| string | 否 | 商品编码
tax_category_name | string | 否 | 税种名称
tax_category_code | string | 否 | 商品英文名称
page | int | 否 | 页码

* **请求示例**
    * http://open_api.aeotrade.com/services/cn_inout_tariff/cn_im_base_rate?auth_key=1111111111&hs_code=1111111111&tax_category_name=xx税&tax_category_code=xxx
* **返回参数类型**
* **返回参数**
* **返回参数示例**


### 3. 出口基本税率
* **请求URL**
    * /services/cn_inout_tariff/cn_ex_base_rate
* **请求类型**
    * GET
* **请求参数**

参数名称 | 参数类型 | 是否必填 | 备注
---|---|---|---
hs_code| string | 否 | 商品编码
tax_category_name | string | 否 | 税种名称
tax_category_code | string | 否 | 商品英文名称
page | int | 否 | 页码

* **请求示例**
* **返回参数类型**
* **返回参数**
* **返回参数示例**


### 4. 进口特惠税率
* **请求URL**
* **请求类型**
* **请求参数**
* **请求示例**
* **返回参数类型**
* **返回参数**
* **返回参数示例**


### 5. 进口协定税率
* **请求URL**
* **请求类型**
* **请求参数**
* **请求示例**
* **返回参数类型**
* **返回参数**
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
* **请求类型**
* **请求参数**
* **请求示例**
* **返回参数类型**
* **返回参数**
* **返回参数示例**


### 3. 报关单单据类型
* **请求URL**
* **请求类型**
* **请求参数**
* **请求示例**
* **返回参数类型**
* **返回参数**
* **返回参数示例**


### 4. 备案清单类型
* **请求URL**
* **请求类型**
* **请求参数**
* **请求示例**
* **返回参数类型**
* **返回参数**
* **返回参数示例**


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
* **请求类型**
* **请求参数**
* **请求示例**
* **返回参数类型**
* **返回参数**
* **返回参数示例**


### 9. 国别地区代码
* **请求URL**
* **请求类型**
* **请求参数**
* **请求示例**
* **返回参数类型**
* **返回参数**
* **返回参数示例**


### 10. 国内地区代码
* **请求URL**
* **请求类型**
* **请求参数**
* **请求示例**
* **返回参数类型**
* **返回参数**
* **返回参数示例**


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
* **请求类型**
* **请求参数**
* **请求示例**
* **返回参数类型**
* **返回参数**
* **返回参数示例**


### 13. 货物属性
* **请求URL**
* **请求类型**
* **请求参数**
* **请求示例**
* **返回参数类型**
* **返回参数**
* **返回参数示例**


### 14. 货物用途
* **请求URL**
* **请求类型**
* **请求参数**
* **请求示例**
* **返回参数类型**
* **返回参数**
* **返回参数示例**


### 15. 集装箱规格
* **请求URL**
* **请求类型**
* **请求参数**
* **请求示例**
* **返回参数类型**
* **返回参数**
* **返回参数示例**


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
* **请求类型**
* **请求参数**
* **请求示例**
* **返回参数类型**
* **返回参数**
* **返回参数示例**


### 19. 企业资质类别
* **请求URL**
* **请求类型**
* **请求参数**
* **请求示例**
* **返回参数类型**
* **返回参数**
* **返回参数示例**


### 20. 检验检疫申请单证代码
* **请求URL**
* **请求类型**
* **请求参数**
* **请求示例**
* **返回参数类型**
* **返回参数**
* **返回参数示例**


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
* **请求类型**
* **请求参数**
* **请求示例**
* **返回参数类型**
* **返回参数**
* **返回参数示例**


### 23. 随附单据类型
* **请求URL**
* **请求类型**
* **请求参数**
* **请求示例**
* **返回参数类型**
* **返回参数**
* **返回参数示例**


### 24. 危包类别
* **请求URL**
* **请求类型**
* **请求参数**
* **请求示例**
* **返回参数类型**
* **返回参数**
* **返回参数示例**


### 25. 危包规格
* **请求URL**
* **请求类型**
* **请求参数**
* **请求示例**
* **返回参数类型**
* **返回参数**
* **返回参数示例**


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
* **请求类型**
* **请求参数**
* **请求示例**
* **返回参数类型**
* **返回参数**
* **返回参数示例**


### 29. 征免性质
* **请求URL**
* **请求类型**
* **请求参数**
* **请求示例**
* **返回参数类型**
* **返回参数**
* **返回参数示例**


### 30. 中国行政区划
* **请求URL**
* **请求类型**
* **请求参数**
* **请求示例**
* **返回参数类型**
* **返回参数**
* **返回参数示例**


## 四、贸易管制商品目录
## 五、贸易单证数据
## 六、其他