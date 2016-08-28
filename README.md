# Ornament/Observer
Observer pattern for Ornament ORM

## Installation

### Composer (recommended)
```sh
$ composer require ornament/observer
```

### Manual
1. Download or clone the repo;
2. Add `/path/to/observer/src` for namespace `Ornament\Observer` to your
   PSR-4 autoloader.

## Usage
For each Model that needs to observe something, let is `use` the
`Ornament\Observer\Observer` trait:

```php
<?php

use Ornament\Observer\Observer;

class ObservingModel
{
    use Observer;
}
```

Similarly, for each Model that needs to be watched, `use` the
`Ornament\Observer\Subject` trait:

```php
<?php

use Ornament\Observer\Subject;

class WatchedModel
{
    use Subject;
}
```


