## 拖拽框的使用

##### 1. 引入js文件

	<script src="js/DragBox.js"></script>

##### 2. 使用


第一步(定义一个放拖拽框的容器):
	
	<div id="container"></div>
	
第二步(定义一个关闭按钮):

	<button id="close">关闭拖拽框</button>	
	
第三步:

	DragBox({
            "width":500,
            "height":500,
            "title":"欢迎登陆",
            "id":"container",
            "closeId":"close"
        });


##### 3. 在拖拽框中加入元素和样式

**首先你的 `CSS` 样式必须要有这一项**

	*{
        margin: 0;
        padding: 0;
     }


**`html ->`**

	<div class="inputBox">
        <div class="contentBox">
            <p><b>姓名:</b><input type="text" value="username"><span>!</span></p>
            <p><b>用户名:</b><input type="text" value="username"><span>!</span></p>
            <p><b>密码:</b><input type="password" value="password"><span>!</span></p>
            <p><b>密码:</b><input type="text" value="username"><span>!</span></p>
            <p><b>邮箱:</b><input type="text" value="username"><span>!</span></p>
            <p><b>手机号:</b><input type="text" value="username"><span>!</span></p>
        </div>
    </div>

**`css ->`**

	*{
            margin: 0;
            padding: 0;
        }
        .inputBox{
            padding-top: 5%;
            width: 100%;
            height: 95%;
        }
        .contentBox{
            width: 60%;
            height: 60%;
            margin: 0 auto;
            text-align: center;
            padding: 10px;
        }

        .contentBox  input{
            width: 200px;
            height: 30px;
            margin: 10px;
            text-indent: 5px;
            border: 1px solid #ccc;
            box-shadow: 0px 0px 4px #ccc;
            outline: none;
        }
        .contentBox  input:focus{
            transition: all 1s ease 0.1s;
            border-color: darkcyan;
            box-shadow: 0px 0px 4px darkcyan;
        }
        .contentBox > p> b{
            display: inline-block;
            width: 60px;
            height: 30px;
            line-height: 30px;
            text-align: center;
        }










