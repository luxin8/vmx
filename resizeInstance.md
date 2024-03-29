## 升级配置

* 综述
  * 本期仅支持升级配置，CPU、内存、SSD数据盘、带宽上限、防御峰值等只允许增加，不允许减少
  * 点击升级配置按钮，当前页面跳转至升级配置页，默认以实例当前配置填充所有项

* 后置条件
  * 升级配置成功则刷新相关字段信息；升级配置失败则浮层提示“云主机XXX升级配置失败”
* 业务规格
  * CPU：
    * 默认选中当前规格的CPU大小
    * 比当前规格CPU小的CPU选项置灰不可选，鼠标移入提示“仅支持升配”
  * 内存：
    * 默认选中当前规格的内存大小
    * 比当前规格内存小的内存选项置灰不可选，鼠标移入提示“仅支持升配”
  * SSD系统盘
    * 选中“免费赠送”，40GB，不可取消选中，右侧问题提示“免费赠送SSD磁盘40GB”
  * SSD数据盘
    * 默认添加当前实例数据盘
    * 已有数据盘可通过拖动或直接输入指定容量：
      * 范围10-1000GB，默认值为已有容量，不支持缩容，仅支持扩容；输入含个位数时向上取整，输入除数字外的其他字符不显示。输入小于原有容量则统一为原有容量，超过1000则统一为1000
      * 已有数据盘不支持删除，删除按钮置灰，鼠标移入提示“不支持删除已有数据盘”
    * 可新增磁盘：
         * 数据盘最多可添加5块，已添加5块后添加按钮置灰不可点
         * 始终显示按钮“+ 添加一块数据盘” 右侧有常显提示【一共可添加 X 块，还可添加 Y 块】
         * 新添加的数据盘可删除
  * 公网IP
    * 勾选框：勾选项名称“随实例购买绑定”，默认勾选，置灰不可取消勾选。
  * 线路
    * BGP
  * 带宽上限
	* 仅支持扩，可通过拖动或直接输入指定，范围1-300Mbps，步长为1，默认值为实例原有上限（不可减小），仅可输入整数，输入小数向上取整，输入除数字外的其他字符不显示。输入小于原有上限则统一为原有上限，超过300则统一为300；
  * 防御峰值：
    * 仅支持扩，可通过拖动或直接输入指定，范围50-300G，步长为10，默认值为原有峰值（不可减小），仅可输入10的倍数，输入个位数向上取整，输入除数字外的其他字符不显示。输入小于原有峰值则统一为原有峰值，超过300则统一为300；
    * 文字提示“中国-香港-12节点 免费提供 50Gbps 的恶意流量攻击防护峰值”
  * 当前配置：展示实例原有计费类型、规格、SSD数据盘、公网带宽、防御峰值、到期时间（样式同主机创建页配置明细）
  * 升级后配置：
    * 展示实例升级后计费类型、规格、SSD数据盘、公网带宽、防御峰值、到期时间、费用（费用为需补差价）
    * 进入页面用户无改动时，展示实例原有配置
  * 立即升配：
    * 页面配置项无改动时，按钮不可点击，鼠标移入提示“所选配置与当前配置相同”
    * 配置项有改动后，按钮可点击，点击进入订单确认页；
  
