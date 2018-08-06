# css开发规范
## 1.代码规范
* 使用stylelint来检查语法规则和代码风格。
* 通过对 stylelint-config-standard 进行扩展，并加入自己的rules。

## 2.stylelint规则列表
"off" 或 0 - 关闭规则
"warn" 或 1 - 开启规则，使用警告级别错误，不会导致程序退出
"error" 或 2 - 开启规则，使用错误级别错误，触发时会导致程序退出
### 颜色
* color-hex-case: 指定十六进制颜色的大小写。
* color-hex-length: 指定十六进制颜色的长度。
* color-named: 在特定的情况下是否允许使用命名的颜色值。
* color-no-hex: 禁止使用十六进制的颜色。
* color-no-invalid-hex: 禁止无效的十六进制颜色。
### 字体系列
* font-family-name-quotes: 指定字体系列是否应用于单双引号内。
### 字体粗细
* font-weight-notation: 要求一致的数值或命名作为
* font-weight 的值。
### 函数
* function-blacklist: 指定一个不允许使用函数的黑名单。
* function-calc-no-unspaced-operator: 禁止在 calc 函数内的运算符间省略空格。
* function-comma-newline-after: 在函数的逗号后指定一个换行符或禁止留有空格。
* function-comma-newline-before: 在函数的逗号前指定一个换行符或禁止留有空格。
* function-comma-space-after: 在函数的逗号后指定一个空格或禁止留有空格。
* function-comma-space-before: 在函数的逗号前指定一个空格或禁止留有空格。
* function-linear-gradient-no-nonstandard-direction: 禁止在 linear-gradient() 内使用不符合 标准语法 的值。
* function-parentheses-newline-inside: 在函数括号内指定一个换行符或禁止留有空格。
* function-parentheses-space-inside: 在函数括号内指定一个空格或禁止留有空格。
* function-url-quotes: 为 urls 指定单引或双引号。
* function-whitelist: 指定一个允许使用函数的白名单。
* function-whitespace-after: 在函数后指定一个空格或禁止留有空格。
### 数值
* number-leading-zero: 要求或不允许数值小于 1 的数字前面添加 0 。
* number-max-precision: 限制数值的小数位数。
* number-no-trailing-zeros: 禁止在数值内尾随 0 。
* number-zero-length-no-unit: 禁止单位长度为 0 。
### 字符串
* string-no-newline: 禁止字符串（非转义）换行。
* string-quotes: 为字符串指定单引或双引号。
### 时长
* time-no-imperceptible: 禁止 animation 与 transition 时长低于 100ms 。
### 单位
* unit-blacklist: 指定一个不允许使用单位的黑名单。
* unit-whitelist: 指定一个允许使用单位的白名单。
### 值
* value-no-vendor-prefix: 禁止值添加供应商前缀。
### 值列表
* value-list-comma-newline-after: 在值列表的逗号后指定一个换行符或禁止留有空格。
* value-list-comma-newline-before: 在值列表的逗号前指定一个换行符或禁止留有空格。
* value-list-comma-space-after: 在值列表的逗号后指定一个空格或禁止留有空格。
* value-list-comma-space-before: 在值列表的逗号前指定一个空格或禁止留有空格。
### 自定义属性
* custom-property-no-outside-root: 禁止 :root 之外的选择器自定义属性。
* custom-property-pattern: 指定自定义属性的模式。
### 属性
* property-blacklist: 指定一个不允许使用属性的黑名单。
* property-no-vendor-prefix: 禁止属性添加供应商前缀。
* property-unit-blacklist: 指定一个特定属性不允许使用单位的黑名单。
* property-unit-whitelist: 指定一个特定属性允许使用单位的白名单。
* property-value-blacklist: 指定一个不允许使用键值对的黑名单。
* property-value-whitelist: 指定一个允许使用键值对的白名单。
* property-whitelist: 指定一个允许使用属性的白名单。
### 声明
* declaration-bang-space-after: 在声明的优先级后指定一个空格或禁止留有空格。
* declaration-bang-space-before: 在声明的优先级前指定一个空格或禁止留有空格。
* declaration-colon-newline-after: 在声明的冒号后指定一个换行符或禁止留有空格。
* declaration-colon-space-after: 在声明的冒号后指定一个空格或禁止留有空格。
* declaration-colon-space-before: 在声明的冒号前指定一个空格或禁止留有空格。
* declaration-no-important: 禁止在声明内使用 !important 。
### 声明块
* declaration-block-no-duplicate-properties: 禁止在声明块内出现重复属性。
* declaration-block-no-shorthand-property-overrides: 禁止使用速记属性重写相关属性。
* declaration-block-properties-order: 指定声明块内属性的顺序。
* declaration-block-semicolon-newline-after: 在声明块的分号后指定一个换行符或禁止留有空格。
* declaration-block-semicolon-newline-before: 在声明块的分号前指定一个换行符或禁止留有空格。
* declaration-block-semicolon-space-after: 在声明块的分号后指定一个空格或禁止留有空格。
* declaration-block-semicolon-space-before: 在声明块的分号前指定一个空格或禁止留有空格。
* declaration-block-single-line-max-declarations: 在单行声明块中限制声明的数量。
* declaration-block-trailing-semicolon: 在声明块内指定或禁止尾随分号。
### 块
* block-closing-brace-newline-after: 在块的右大括号后指定一个换行符或禁止留有空格。
* block-closing-brace-newline-before: 在块的右大括号前指定一个换行符或禁止留有空格。
* block-closing-brace-space-after: 在块的右大括号后指定一个空格或禁止留有空格。
* block-closing-brace-space-before: 在块的右大括号前指定一个空格或禁止留有空格。
* block-no-empty: 禁止空块。
* block-no-single-line: 禁止单行块。
* block-opening-brace-newline-after: 在块的左大括号后制定一个换行符。
* block-opening-brace-newline-before: 在块的左大括号前指定一个换行符或禁止留有空格。
* block-opening-brace-space-after: 在块的左大括号后指定一个空格或禁止留有空格。
* block-opening-brace-space-before: 在块的左大括号前指定一个空格或禁止留有空格。
### 根选择器
* root-no-standard-properties: 禁止使用标准属性内的 :root 选择器。
### 选择器
* selector-class-pattern: 指定类选择器的模式（模式指的是正则表达式）。
* selector-combinator-space-after: 在复合选择器之后要求或不允许留有一个空格。
* selector-combinator-space-before: 在复合选择器之前要求或不允许留有一个空格。
* selector-id-pattern: 指定 id 选择器的模式。
* selector-max-specificity: 限制选择器的特异性。
* selector-no-attribute: 禁止属性选择器。
* selector-no-combinator: 禁止复合选择器。
* selector-no-id: 禁止 id 选择器。
* selector-no-type: 禁止类型选择器。
* selector-no-universal: 禁止通用选择器。
* selector-no-vendor-prefix: 禁止选择器添加供应商前缀。
* selector-pseudo-element-colon-notation: 为伪元素指定适当的单或双冒号。
* selector-root-no-composition: 禁止复合 :root 选择器。
### 选择器列表
* selector-list-comma-newline-after: 在选择器列表的逗号后指定一个换行符或禁止留有空格。
* selector-list-comma-newline-before: 在选择器列表的逗号前指定一个换行符或禁止留有空格。
* selector-list-comma-space-after: 在选择器列表的逗号后指定一个空格或禁止留有空格。
* selector-list-comma-space-before: 在选择器列表的逗号前指定一个空格或禁止留有空格。
### 规则
* rule-nested-empty-line-before: 要求或不允许嵌套规则前留有空行。
* rule-non-nested-empty-line-before: 要求或不允许非嵌套规则前留有空行。
### 媒体特性
* media-feature-colon-space-after: 在媒体特性的冒号后指定一个空格或禁止留有空格。
* media-feature-colon-space-before: 在媒体特性的冒号前指定一个空格或禁止留有空格。
* media-feature-name-no-vendor-prefix: 禁止媒体特性属性名添加供应商前缀。
* media-feature-no-missing-punctuation: 确保非布尔型媒体特性具有所需的标符：一个冒号或范围运算符。
* media-feature-range-operator-space-after: 在媒体特性的范围运算符后指定一个空格或禁止留有空格。
* media-feature-range-operator-space-before: 在媒体特性的范围运算符前指定一个空格或禁止留有空格。
### 自定义媒体
* custom-media-pattern: 指定自定义媒体查询的名称模式。
### 媒体查询
* media-query-parentheses-space-inside: 在媒体查询括号内要求或不允许留有一个空格。
### 媒体查询列表
* media-query-list-comma-newline-after: 在媒体查询列表的逗号后指定一个换行符或禁止留有空格。
* media-query-list-comma-newline-before: 在媒体查询列表的逗号前指定一个换行符或禁止留有空格。
* media-query-list-comma-space-after: 在媒体查询列表的逗号后指定一个空格或禁止留有空格。
* media-query-list-comma-space-before: 在媒体查询列表的逗号前指定一个空格或禁止留有空格。
### AT规则
* at-rule-empty-line-before: 在 AT规则 前要求或不允许留有空行。
* at-rule-no-vendor-prefix: 禁止 AT规则 添加供应商前缀。
### 注释
* comment-empty-line-before: 要求或不允许注释前面留有一个空格。
* comment-whitespace-inside: 要求或不允许注释内留有一个空格。
### 常用样式
* indentation: 指定缩进。
* max-empty-lines: 限制相邻的空行数。
* max-line-length: 限制每行的长度。
* max-nesting-depth: 限定嵌套深度。
* no-browser-hacks: 禁止使用与目标的浏览器无关的 CSS hack。
* no-descending-specificity: 禁止特异性较低的选择器在特异性较高的选择器之后重写。
* no-duplicate-selectors: 禁止使用重复的选择器。
* no-eol-whitespace: 禁止行尾留有空白。
* no-indistinguishable-colors: 禁止使用极其相似的颜色。
* no-invalid-double-slash-comments: 禁止使用 CSS 不支持的双斜线注释 (//...) 。
* no-missing-eof-newline: 要求文件结尾留有换行符。
* no-unknown-animations: 禁止 animation 使用 与 @keyframes 声明不对应的名称。
* no-unsupported-browser-features: 禁止使用目标浏览器不支持的属性。