    •	Leon Li ClaClo-Admin
	•	Silvio Zheng ClaClo-Teacher
	•	Shawn Cui (Team Leader) ClaClo-Manager  
	•	Yunxiang Wang ClaClo-Student


# 课程作业规范
---

#### 1. 被评估的学习成果

本课程作业占该模块总评估的100%。旨在评估以下学习成果的达成情况：
1. 展示对软件生命周期的理解，并能够对问题进行批判性分析，从而决定适用的流程模型。
2. 展示对项目风险的理解，并能够识别和管理项目中的风险和变化影响。
3. 展示对需求分析和引导的理解，以及需求与设计之间的关系，并能够为项目创建功能性和非功能性需求。
4. 能够批判性地评估和利用面向对象分析和设计、基于组件设计以及面向服务的设计的设计范式。
5. 描述并运用软件技术，通过实现设计来实现包括可靠性、效率和鲁棒性在内的预期软件质量。
6. 了解并能够应用各种测试方法和技术。
7. 在修改软件组件的过程中使用重构。
8. 了解软件可靠性如何对系统可靠性做出贡献，并能够应用多种方法来开发软件系统的可靠性估计。

---

#### 2. 需要解决的问题

在本课程作业中，您需要组成一个由四名学生组成的软件工程团队，应用适当的软件工程方法和技术来开发一个指定的现代计算机应用系统（本课程作业不要求编写代码）。团队中的每个成员都将进行软件工程活动以开发一个子系统，并与团队其他成员合作，确保这些子系统集成并相互作用，从而形成一个一致的系统。具体应用的简要描述可在模块的Moodle网站上找到的文件COMP6030-CW-Case Study中查看。

您需要完成第3节中指定的一系列软件工程任务，并生成一组软件工程文档，以证明：
- (a) 您理解软件工程方法论的原则，
- (b) 您能够选择和应用适当的软件工程技术，
- (c) 您具备使用高级软件工程工具的技能。

---

#### 3. 需要完成的任务

以下是本课程作业中需要完成的任务以及评分分布。更详细的评分标准可以在模块的Moodle网站上找到的文件COMP6030-CW-Detailed Marking Scheme中查看。

- **任务0：团队组织和项目管理**  
  学生需要自行组建一个由四名学生组成的团队。团队必须建立一个管理方案和协作机制，并在整个学期中密切合作。  
  每个团队必须为课程作业项目设置一个GitHub存储库，以托管项目文件。  
  团队必须定期（例如每周至少一次）在固定的日期和时间举行会议。每次会议之前应有议程，会议应记录内容，尤其是出席情况、进展、待办事项清单以及待解决的问题。会议议程和记录应在创建后立即上传到GitHub。  
  每个课程作业团队成员必须负责开发以下子系统之一：
    - (a) **ClaClo-Student**：用于学生接收信息和学习资料，并进行练习和/或提交评估工作。
    - (b) **ClaClo-Teacher**：用于教师给学生布置练习和作业，接收并批改学生作品（包括练习和评估），并向学生提供反馈。
    - (c) **ClaClo-Admin**：用于课程管理员的子系统。
    - (d) **ClaClo-Manager**：用于大学管理人员管理课程的子系统。

  注意：团队成员应负责不同的子系统，同时整个团队应开发一个一致的系统，子系统之间能够相互作用。每个子系统必然包含两部分：一部分在用户的计算机或移动设备上运行，另一部分在云端服务器上运行。属于不同子系统的云端部分应进行适当集成，以便它们相互作用，为不同类型的用户提供功能。此外，还可能存在在云端运行的组件，这些组件可能为多个子系统共享或不属于任何特定子系统。团队还应共同开展软件工程活动以开发此类共享组件。

- **任务1：软件功能需求的规范与建模 (20分)**  
  在此任务中，您将作为项目中的需求分析师，使用软件建模工具生成待开发软件系统的UML模型。UML模型应包含以下模型类型。
    - (a) **用例模型 (10分，个人任务)**：团队中的每位成员应开发一个用例图，定义子系统的用例，以明确软件工程项目的范围。
    - (b) **活动模型 (10分，个人任务)**：每位团队成员应选择一个子系统的用例，生成该用例的活动图，以指定用户与子系统之间的交互。

- **任务2：软件架构设计 (30分)**  
  在此任务中，您将作为软件架构师，以微服务架构风格生成系统的架构设计。设计应包含两个不同抽象级别：
    - (a) **子系统架构 (15分，个人任务)**：每位团队成员应生成其子系统的架构设计，关注子系统提供的微服务以及子系统请求和其他子系统提供的微服务。
    - (b) **整个系统的架构 (15分，团队任务)**：团队应通过集成各子系统来生成整个系统的架构设计。

  注意：
    - 您应在UML组件图中指定架构设计，其中包含用于表示微服务的组件节点和用于表示连接器的接口。
    - 应以文本形式指定组件和连接器，包括其方法和参数，以定义其功能和含义。
    - 在此设计部分中，不需要给出组件和连接器的内部结构。

- **任务3：软件详细设计 (20分)**  
  在此任务中，您将作为软件设计师，生成系统的详细设计，以便面向对象地实现子系统架构设计中的组件（即微服务）。设计应从结构和行为两个方面指定组件的内容。
    - (a) **结构模型 (10分，个人任务)**：每位学生应选择子系统架构设计中的一个组件，并开发该组件的类图，以定义其结构。
    - (b) **行为模型 (10分，个人任务)**：每位学生应为任务3(a)中选择的相同组件生成一个序列图，以定义该组件的动态行为。

- **任务4：软件测试 (30分)**  
  在此任务中，您将作为软件质量工程师开发一个软件测试计划。您的测试计划应包含两部分：
    - (a) **单元测试计划 (15分，个人任务)**：您应选择子系统中的一个微服务，开发该微服务的单元测试计划。
    - (b) **系统测试计划 (15分，个人任务)**：您应选择一个用例，开发该用例的系统测试计划。

---

#### 4. 课程作业提交

- **4.1 何时提交**  
  提交截止日期为2024年12月6日（周五）晚23:00（第11周）。

- **4.2 提交内容**  
  每个小组应提交一个压缩文件（zip），该文件包含以下文件表中列出的文件。文件名及其内容应遵循表中的约定。

- **4.3 提交地点**  
  您必须将包含所有组件的zip文件上传至模块的Moodle网站。


# 课程案例研究文档：
---

### **1. 简介**
随着移动计算和云计算技术的兴起，人们认为可以开发出新一代的虚拟学习环境，以全面支持大学的教学和学习，同时通过利用诸如软件即服务（Software-as-a-Service, SaaS）等信息技术实现大学运营的自动化。CloudSoft Ltd（一个虚构的公司，专门开发计算机应用系统）决定开发一个名为ClaClo的系统。该系统是一个多租户在线平台，旨在实现教学、学习、课程管理和运营的高级功能。每个租户应为一个教育机构，例如一所大学。

本文档定义了该系统的功能需求。文档的其余部分组织如下：**第2部分**定义了目标用户类型；**第3部分**介绍了系统的关键设计特性；**第4至第6部分**列出了根据用户类型划分的ClaClo系统的功能需求。

---

### **2. 目标用户类型**
系统的主要用户类型包括以下几类：
(a) **学生**：指平台上大学的学生，他们将使用移动应用程序和/或桌面计算机参与大学提供的课程学习。  
(b) **教师**：指大学的教学人员，他们将使用桌面计算机上传教学材料，与学生和课程管理员进行沟通。  
(c) **机构管理者**：通常为大学学术管理部门的工作人员，他们将使用桌面计算机通过输入和更新大学相关数据来设置、定制和更新机构的站点。  
(d) **部门管理员**：通常为大学部门的行政工作人员，负责管理和执行大学某部门所提供课程的行政任务。  
(e) **系统操作员**：指平台的运营人员，他们将使用桌面计算机管理租户大学，并为其提供服务。

---

### **3. 关键设计特性**
ClaClo 系统预计由以下子系统组成，这些子系统连接到云端运行的服务上：  
(a) **ClaClo-Student**：为学生提供接收信息和学习材料、完成练习以及提交评估作品的子系统。  
(b) **ClaClo-Teacher**：为教师提供布置练习和作业、接收和评分学生作业并提供反馈的子系统。  
(c) **ClaClo-Admin**：为课程管理员提供的子系统。  
(d) **ClaClo-Manager**：为大学管理者提供管理大学课程的子系统。  
(e) **ClaClo-Ops**：为平台操作员提供管理租户大学账户并提供跨大学服务的子系统。

---

### **4. 功能需求规范**

#### **4.1. 大学管理者的需求**
**FR-IM-1**：**管理大学账户**  
系统应支持大学管理者设置（或定制）和更新大学账户的相关数据，账户应包括以下信息：
- **学位项目**：包括大学提供的学位项目列表及相关文件；
- **大学部门**：包括部门名称以及各部门提供的学位项目。

**FR-IM-2**：**管理学生记录**  
系统应支持大学管理者管理学生记录，包括学生的学习计划（如修读的课程及时间）和学术表现。

**FR-IM-3**：**查看学生记录变更的痕迹**  
所有对学生记录的操作必须被永久记录并存档，用于审计目的。系统应支持大学管理者搜索并查看学生记录变更的痕迹。

**FR-IM-4**：**管理行政人员记录**  
系统应支持大学管理者管理每个部门的行政人员账户，包括创建、更新及删除或存档相关记录。

---

---

# 评分标准：
---

#### **任务 1：软件建模与规范**
**总分：20 分**

- **(a) 用例模型** *(个人评分，10 分)*
  - (a) 图表必须语法正确。
  - (b) 用例模型必须完整，涵盖所有需求。
  - (c) 用例之间的关系必须语义正确。
  - (d) 用例必须处于适当的抽象层次。
  - (e) 用例模型必须清晰地定义系统范围。

- **(b) 活动模型** *(个人评分，10 分)*
  - (a) 活动图必须表示用户类型与系统之间的交互。
  - (b) 必须使用泳道图（Swimlane）来指明谁在执行什么任务。
  - (c) 必须在图表中呈现对象流，以指定不同活动之间传递的数据。
  - (d) 图表必须在语法和语义上正确。
  - (e) 图表必须与需求定义和用例模型一致。

---

#### **任务 2：软件架构设计**
**总分：15 分**

- **(a) 子系统的架构** *(个人评分，15 分)*
  - (a) 子系统的架构设计必须以 UML 组件图形式呈现，且在语法和语义上正确。
  - (b) 架构设计必须符合微服务架构风格。
  - (c) 设计必须与整个系统的总体架构一致。
  - (d) 设计必须与需求保持一致且完整。
  - (e) 文本规范必须与图表一致。

- **(b) 整个系统的架构** *(团队评分，15 分)*
  - (a) 整个系统的结构必须以 UML 组件图形式表示，且在语法和语义上正确。
  - (b) 架构设计必须符合微服务架构风格。
  - (c) 每个团队成员的子系统部分必须一致整合，不应有重复或不必要的重叠。
  - (d) 系统的设计必须与需求定义一致。
  - (e) 文档必须清楚地定义组件和连接器的功能。  
    **注**：如果团队成员未对团队部分做出贡献，则不会获得团队分数。

---

#### **任务 3：软件详细设计**
**总分：20 分**

- **(c) 结构模型** *(个人评分，10 分)*
  - (a) 必须以 UML 类图形式表示选定组件的结构，语法和语义正确。
  - (b) 选定的组件必须属于你负责的子系统，而非其他子系统，且不能是琐碎组件。
  - (c) 模型必须完整，没有明显遗漏重要的类及其关系。
  - (d) 模型必须足够详细，包括属性和方法，以支持后续开发。
  - (e) 模型必须与组件功能以及架构设计中指定的接口一致。

- **(d) 行为模型** *(个人评分，10 分)*
  - (a) 序列图必须对应任务 3(a) 中的同一组件。
  - (b) 模型必须与架构设计中该组件的定义一致。
  - (c) 模型必须以 UML 序列图形式表示，且语法和语义正确。
  - (d) 必须使用高级 UML 序列图语言功能，如重复框架、备选框架等。
  - (e) 序列图必须完整，包含重要的信息，如消息参数、守卫条件等。

---

#### **任务 4：软件测试**
**总分：30 分**

- **(a) 单元测试计划** *(个人评分，15 分)*
  - (a) 单元测试计划用于测试子系统中的一个微服务。
  - (b) 测试计划必须与子系统的架构一致。
  - (c) 测试计划必须与组件的详细设计一致。
  - (d) 测试计划必须覆盖所有方法、属性以及组件在不同操作条件下的表现。
  - (e) 测试计划必须足够详细，以便测试人员执行。

- **(b) 系统测试计划** *(个人评分，15 分)*
  - (a) 系统测试计划用于测试子系统中的一个选定用例。
  - (b) 测试计划必须与需求定义以及用例和活动模型一致。
  - (c) 测试计划必须覆盖用例的所有可能场景。
  - (d) 测试计划必须覆盖设计模型中规定的系统内部所有可能行为。
  - (e) 测试计划必须足够详细，以便测试人员执行。

---

### **总分**
- 团队评分：15 分
- 个人评分：85 分

