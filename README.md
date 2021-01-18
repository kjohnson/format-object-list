# Format Object List

Formats an associative array into a JS parsable array of label/value objects.

## Usage

```php
$data = [ 'foo' => 'bar' ];
$formatter = FormatObjectList\Factory::fromKeyValue( $data );
$list = $formatter->format();
// [ [ 'label' => 'bar', 'value' => 'foo' ] ]
```

```php
$data = [ 'foo' => 'bar' ];
$formatter = FormatObjectList\Factory::fromValueKey( $data );
$list = $formatter->format();
// [ [ 'label' => 'foo', 'value' => 'bar' ] ]
```
