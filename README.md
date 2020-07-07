# 拖延症如何解决

1. 五分钟学习法
2. 仪式感
3. 有区别的拖延
4. 认清自己（照照镜子：高吗？帅吗？富吗？）

# 文件的删除操作

* 删除文件：`rm 1.txt`
* 删除文件夹：`rm -r a`

# 这是一段代码

```javascript
		<script>
			
			var TodoItem = {
				props: ['content', 'index'],
				template: "<li @click='handleItemClick'>{{content}}</li>",
				methods: {
					handleItemClick: function(){
						this.$emit("delete", this.index);
					}
				}
			}
			
			var app = new Vue({
				components: {
					TodoItem: TodoItem
				},
				el: '#app',
				data: {
					list: [],
					inputValue: ''
				},
				methods: {
					handleBtnClick: function(){
						this.list.push(this.inputValue)
						this.inputValue = ''
					},
					handleItemDelete: function(index){
						this.list.splice(index, 1);
					}
				}
			})
		</script>
```
