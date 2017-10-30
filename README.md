# authority
http://es6.ruanyifeng.com/#docs/let  ES6
Redux 核心概念介绍
从上述的图中我们可以看到 Redux 资料流的模型大致上可以简化成： View -> Action -> (Middleware) -> Reducer。当使用者和 View 互动时会触发事件发出 Action，若有使用 Middleware 的话会在进入 Reducer 进行一些处理，当 Action 进到 Reducer 时，Reducer 会根据，action type 去 mapping 对应处理的动作，然后回传回新的 state。View 则因为侦测到 state 更新而重绘页面。在这个章节我们讨论的是 synchronous（同步）的情形，asynchronous（非同步）的状况会在接下来的章节进行讨论。以下就用官方网站上的简单范例来让大家感受一下 Redux 的整个使用流程：

总之 Redux 提供了：	
	// 1）存放应用程序状态的容器
	// 2）一种把 action 分发到状态修改器的机制，也就是 reducer 函数
	// 3）监听状态变化的机制

combineReducers 接收一个对象并返回一个函数，当 combineReducers 被调用时，它会去调用每个 reducer，并把返回的每一块 state 重新组合成一个大 state 对象（也就是 Redux 中的 Store）。
Dispatch用来分发action  然后通过reducer 函数修改应用状态
action ---> dispatcher ---> middleware 1 ---> middleware 2 ---> reducers

/*
    var anyMiddleware = function ({ dispatch, getState }) {
        return function(next) {
            return function (action) {
                // 你的中间件业务相关代码
            }
        }
    }
*/
redux 介绍
https://github.com/react-guide/redux-tutorial-cn
https://developer.mozilla.org/zh-CN

JavaScript 全栈工程师培训教程 阮一峰
https://github.com/ruanyf/jstraining/tree/master/docs


http://www.bootcss.com/ 中文网站
算法
http://blog.jobbole.com/67348/
高性能javascript
https://mzkmzk.gitbooks.io/read/content/gao_xing_neng_javascript.html
