Changelog
=========

### 1.3.0
- Started keeping a log of all changes between releases
- Added support for quickly exposing functions as cli clients with `hug.cli` decorator
- Added support for quickly serving up development APIs from withing the module using: `if __name__ == '__main__': __hug__.serve()
- Added support for documentation only type annotations, simply by passing just a string in as the type annotation
- Added support for `requires` argument to limit execution of functions based on a given criteria
- Added automatic documentation of output type transformations
- Added initial built-in authentication support
- Added built-in support for outputting common image file types
- Added support for returning streams within hugged functions
- `hug.types.decimal` renamed to `hug.types.float_number` and `hug.types.decimal` type added that returns python Decimal
- `hug.types.accept` wrapper added, that makes it easy to customize doc strings and error handling for any preexisting type converter

### 1.3.1
- Fixed string only annotations causing exceptions when used in conjunction with `hug.cli`
- Fixed return of image file not correctly able to set stream len information / not correctly returning with PIL images
- Added examples of image loading with hug
