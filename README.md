# angular-snippets

Clone this repo into your sublime user folder. Type the trigger(e.g. a-fact) and press tab to create the snippet. Use tab to edit the next field.

##Installation
Linux:
```
cd "~/.config/sublime-text-3/Packages/User"
git clone https://github.com/Dema1348/angular-snippets.git
```


Mac: 
```
cd ~/Library/Application\ Support/Sublime\ Text\ 3/Packages/User
git clone https://github.com/Dema1348/angular-snippets.git
```


Windows:
```
cd "C:/Users/%NAME%/AppData/Roaming/Sublime Text 3/Packages/User"
git clone https://github.com/Dema1348/angular-snippets.git
```

## Examples
```
a.mod

(function() {
	angular.module('${1:app}', [$2]);
})();

```

```
a.ctr

(function() {
  'use strict';

  angular
    .module('${1:app}')
    .controller('${2}', ${2});

  $2.\$inject = [];

  function ${2}() {
    var vm = this;

    ${3}
  }

})();
```

```
a.fac

(function() {
	'use strict';

	angular
    .module('${1:app}')
 	 .factory('${2}Factory', ${2}Factory);

  ${2}Factory.\$inject = [];

	function ${2}Factory(${3}) {
    var services = {
      ${4}: ${4},
    };

    return services;

    function ${4}(${5}) {
      ${6}
    }
	}

})();
```

```
a.dir

(function() {
	'use strict';

	angular
    .module('${1:app}')
	  .directive('${2}', ${2});

	function ${2}() {
    var directive = {
      template: '',
      link: link
    };

    return directive;

    function link(scope, elem, attrs) {
      ${3}
    }
	}

})();
```
