# wp-node_hooks
## a documentation of what it does

This module was adapted from one of wp developer’s discussion. The discussion was about creating the same hook environment as it’s PHP counterpart in Javascript. With that said, let’s test it out. I’ve already tried to salvage its methods, so that it can be accessed through simple requires.

## Functions
```javascript
var hooks = require( ‘node-wp_hooks’ );

// By doing this in a document, you can access all aforementioned hooks. The following are methods of the object.

// Actions
hooks.doAction(  action, args  );
hooks.addAction( action, callback, priority, context );
hooks.removeAction( action, callback );

// Filters
hooks.applyFilters( filter, args );
hooks.addFilter(  filter, callback, priority, context  );
hooks.removeFilter( filter, callback );

// Utility
hooks.reload();
```
