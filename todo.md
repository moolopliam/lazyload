# TODO

## Coming next

-   Consider removing the `delay_load` option, there's now a better way to do that. Open an issue to ask the community.
-   Consider not using the `load` event listener for videos.
-   Update the `destroy` method so it also removes lazyload's modifications to DOM elements (`element.llStatus` and `element.llTimeout`)
-   When `cancel_on_exit` is `false`, unobserve elements as soon as they start loading (as of before 15.2.0).
-   Try setting the status inside the element using `element.llStatus` and `element.llTimeout` instead of using DOM attributes `data-ll-status` and `data-ll-timeout`? It would be more protected so harder to hack, and probably faster to read and write.
-   Check how LazyLoad behaves when a page was updated using DOM morphing.
    If only the data-attributes were updated, how do one forces LazyLoad to read from them again?

## Test

-   Test more modules and functions, coverage!!!
-   Test native `img`, native `iframe`, alone or in conjunction with `video`s.

Test more modules

-   [ ] autoinitialize
-   [ ] purge
-   [ ] reveal
