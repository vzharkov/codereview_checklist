# Simple code review checklist

# Before code review hook:
  - Read specification or issue description to understand what problem solve this PR.

# Review body:

* DB migration safety:
  - rollback ability;
  - index missed / extra index;
  - look for possible table locks;
  - quote time needed for migration;
  - move data migration to better place(rake task/ seeds) if it possible;
  
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

* Production safety:
  - deploy plan and it's safety;
  - what related mobules can be corrupted.

# After code review hook:
  - Read all review comments before click "Submit review" btn.
  - Check ability to apply lazy refactoring for the feature. (create external issue to fix technical debt in future if it possible and not critical)
