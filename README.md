# Simple code review checklist

* DB migration safety:
  - rollback ability;
  - index missed / extra index;
  
* Templates:
  - html_safe presence;
  - logic in templates;

* Code safety:
  - N+1 queries;
  - object(that is nil).call;

* Semantic naming:
  - classes/modules;
  - variables/constants;
  
* Code style:
  - simplisity;
  - domain logic design;
