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
  
* Rails Controllers:
  - `find_by!` for record search;
  - authorization checks;
  - less logic amount in controllers;

# After code review hook:
  - Check ability to apply lazy refactoring for the feature. (create external issue to fix technical debt in future if it possible and not critical)
