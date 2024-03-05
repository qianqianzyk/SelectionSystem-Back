# 德育导师双向选择系统

本项目报告详细介绍了德育导师双向选择系统的设计与实现。该系统旨在优化学生和导师之间的选择过程，提高匹配效率。系统支持学生、教师和管理员三种角色，各自有不同的权限和功能。学生可以填写个人信息、选择导师、发送私信和提建议；教师可以审批学生请求、设置审批时间、回复私信和查看最终学生名单；管理员则负责设置截止时间、重置密码、查看双向选择表和审批学生请求。
系统采用MySQL数据库存储数据，包含用户表、教师表、学生表、理由表、私信表、截止时间表和建议表。通过条件判断和状态转移算法，实现了学生选择导师、教师审批、学生填写双向选择表以及管理员审批的流程。
在设计模式上，系统采用了模型-视图-控制器（MVC）架构，以提高代码的可维护性和扩展性。模型负责业务逻辑和数据处理，视图展示数据，控制器处理用户请求并调度模型和视图。
项目面临的主要难点包括跨域问题和定时器处理。跨域问题通过在服务器设置CORS头部定时器则通过robfig/cron库实现，以在规定时间自动分配学生给老师。
总的来说，本项目功能完备、设计合理，旨在通过系统化管理提高学生和导师选择的效率和质量。
