# summernote-grid

A [Summernote](https://summernote.org/) plugin that adds a button to the toolbar allowing the user to create custom grid columns.

See [example.](https://rawgit.com/perevoshchikov/summernote-grid/master/example/index.html)



## Usage

``` html
<script src="https://cdn.jsdelivr.net/gh/perevoshchikov/summernote-grid@1.0.0/summernote-grid.min.js"></script>

<script type="text/javascript">
    $(document).ready(function() {
        $('.summernote').summernote({
            toolbar:[
                ['insert', ['grid']]
            ]
        });
    });
</script>
```

## Full options
```javascript
$('.summernote').summernote({
    toolbar:[
        ['insert', ['grid']]
    ],
    grid: {
        wrapper: "row",
        columns: [
            "col-md-12",
            "col-md-6",
            "col-md-4",
            "col-md-3",
        ]
    },
    callbacks: {
        onGridInsert: null
    },
    icons: {
        grid: "glyphicon glyphicon-th"
    }
});
```

## i18n
```javascript
$.extend($.summernote.lang, {
    'en-US': {
        grid: {
            tooltip: "Columns",
            label: "Columns",
        }
    }
});
```

## License

The MIT License (MIT). Please see [License File](LICENSE.md) for more information.