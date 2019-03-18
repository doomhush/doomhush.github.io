# java实用代码集

## 主动抛出异常
在自定义的错误出现时，想跳转到友好的提示页面，除了代码主动抛出，还需要在web.xml里面增加该异常代码对应的页面
```
// java代码
response.sendError(999);

// web.xml配置
<error-page>
  <error-code>999</error-code>
  <location>/WEB-INF/jsp/common/error/error999.jsp</location>
</error-page>
```
