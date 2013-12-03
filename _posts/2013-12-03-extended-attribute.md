---
layout: post
title:  "扩展属性"
date:   2013-12-03 14:01:09
---

扩展属性是指在数据中附加的除了表单原本字段对应值以外的用于扩展的值，可能是任意一个数据，比如微信的OpenID。

使用时，需要在发布出去的表单URL中传入名为x_field_1的参数，如`https://jinshuju.net/f/A1B2C3?x_field_1=654321`，那么654321即为名为x_field_1的扩展属性。

通过包含扩展属性的链接提交的数据将保存该属性，并会在数据列表页面、数据详情页面及导出的Excel中展示出来，[数据推送](/http-push.html)时也会包含该属性。

扩展属性只用于透明传输，不会作为普通字段显示在表单中，金数据不对其值进行任何处理和转换，亦不参与过滤和报表运算。

金数据最多可以支持1个扩展属性，并要求使用扩展属性的表单的创建人当前必须拥有金数据标准版套餐及以上。