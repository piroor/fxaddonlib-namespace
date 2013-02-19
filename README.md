# Shared Namespace Library for JavaScript Code Modules

## Usage

    Components.utils.import('resource://my-modules/namespace.jsm');
    var namespace = getNamespaceFor('mylibrary');
    if (!namespace.func1) {
      namespace.func1 = function() { ... };
      namespace.func2 = function() { ... };
    }
    var EXPORTED_SYMBOLS = ['func1', 'func2'];
    var func1 = namespace.func1;
    var func2 = namespace.func2;

