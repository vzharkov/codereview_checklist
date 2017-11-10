# Simple code review checklist

* DB migration safety:
  - rollback ability;
  - index missed / extra intex;
  
* Templates:
  - html_safe presence;
  - logic in templated;

* N+1 queries
* object(that is nil).call
