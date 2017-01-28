Widget Types
============

Plugins can supply custom widget types for the Dashboard by supplying a class that implements `craft\base\WidgetInterface`.

As a convenience, widget classes can extend `craft\base\Widget`, which provides a base implementation of the interface.

You can refer to Craft’s own widget classes for examples. They are located in `vendor/craftcms/cms/src/widgets/`.

## Registering Custom Widget Types

Once you have created your widget class, you will need to register it with the Dashboard service, so Craft will know about it when populating the list of available widget types: 

```php
<?php
namespace ns\prefix;

use craft\events\RegisterComponentTypesEvent;
use craft\services\Dashboard;

class Plugin extends \craft\base\Plugin
{
    public function init()
    {
        Event::on(Dashboard::class, Dashboard::EVENT_REGISTER_WIDGET_TYPES, function(RegisterComponentTypesEvent $event) {
            $event->types[] = MyWidget::class;
        });

        // ...
    }

    // ...
}
```