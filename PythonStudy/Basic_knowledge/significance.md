一、接口测试的必要性和意义

接口，即API，应用程序编程接口

这里主要说说接口测试的必要性和意义：

接口测试实施在多系统的平台架构下，有着极为高效的成本收益比（当然，单元测试收益更高，但实施单元测试的成本投入更大，技术要求更高，所以应该选择更适合自身的才是最好的方案）。

接口测试天生为高复杂性的平台带来高效的缺陷检测和质量监督能力，平台复杂，系统越庞大，接口测试的效果越明显。

总的来说，接口测试是保证高复杂性系统质量的内在要求和低成本的经济利益驱动作用下的最佳方案，主要体现在如下三个方面：

1、节省了测试成本

   根据数据模型推算，底层的一个程序BUG可能引发上层的8个左右BUG，而且底层的BUG更容易引起全网的死机；接口测试能够提供系统复杂度上升情况下的低成本高效率的解决方案。

2、接口测试不同于单元测试

   接口测试是站在用户的角度对系统接口进行全面高效持续的检测。

3、效益更高

   将接口测试实现为自动化和持续集成，当系统复杂度和体积越大，接口测试的成本就越低，相对应的，效益产出就越高。

 

二、做接口测试需要哪些技能

做接口测试，需要的技能，基本就是以下几点：

业务流：了解系统及内部各个组件之间的业务逻辑交互；

数据流：了解接口的I/O（input/output：输入输出）；

协议：包括http协议，TCP/IP协议

工具：工具可以辅助我们更好更高效的完成工作，常用的接口测试工具有：jmeter、loadrunner、soapui、postman等；

数据库知识：无论是从数据库获取知识，还是确认数据落地，抑或接口对数据执行了哪些操作，都需要确认，因此数据库知识（其实就是增删改查）就很有必要；

补充：接口文档的几个必要点：完整性、一致性、容错性；

 

三、接口自动化测试

1、如何开展

首先，调试单个接口，保证单个接口的正确和通畅（类似于性能测试中的基准测试）；

其次，明确数据流，业务流；

最后，将N个接口测试脚本串起来，执行即可；

最重要的一点，别想太多太复杂，先把最基础最简单的做起来，就成功一大半了，至于扩展性的第三方接口、https、定时任务、自动出测试报告、自动发邮件等等功能，这都是不断累计和优化的，

行动起来就行，想太多不如行动起来，让接口自动化测试落地，才是我们首先需要考虑的！

2、开展之前需要知道的

现在的测试对象包含几个页面？

每个页面涉及几个接口？

分别在哪一步调用？

每个接口包含哪些字段？

各个字段对应数据库哪张表？

每个表中各个字段是什么意思？

各个接口对表产生了怎样的操作？

3、自动化框架(python)
Python+unittest(pytest)+requests+HTMLTestRunner(学习推荐)
Robot Framework
httprunner
Vue + Flask
