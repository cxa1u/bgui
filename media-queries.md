/* Extra small devices (phones, less than 768px) */
/* No media query since this is the default in Bootstrap */

/* Small devices (tablets, 768px and up) */
@media (min-width: @screen-sm-min) { ... }

/* Medium devices (desktops, 992px and up) */
@media (min-width: @screen-md-min) { ... }

/* Large devices (large desktops, 1200px and up) */
@media (min-width: @screen-lg-min) { ... }


@media (max-width: @screen-xs-max) { ... }
@media (min-width: @screen-sm-min) and (max-width: @screen-sm-max) { ... }
@media (min-width: @screen-md-min) and (max-width: @screen-md-max) { ... }
@media (min-width: @screen-lg-min) { ... }


//== Media queries breakpoints
//
//## Define the breakpoints at which your layout will change, adapting to different screen sizes.

// Extra small screen / phone
//** Deprecated `$screen-xs` as of v3.0.1
$screen-xs:                  480px !default;
//** Deprecated `$screen-xs-min` as of v3.2.0
$screen-xs-min:              $screen-xs !default;
//** Deprecated `$screen-phone` as of v3.0.1
$screen-phone:               $screen-xs-min !default;

// Small screen / tablet
//** Deprecated `$screen-sm` as of v3.0.1
$screen-sm:                  768px !default;
$screen-sm-min:              $screen-sm !default;
//** Deprecated `$screen-tablet` as of v3.0.1
$screen-tablet:              $screen-sm-min !default;

// Medium screen / desktop
//** Deprecated `$screen-md` as of v3.0.1
$screen-md:                  992px !default;
$screen-md-min:              $screen-md !default;
//** Deprecated `$screen-desktop` as of v3.0.1
$screen-desktop:             $screen-md-min !default;

// Large screen / wide desktop
//** Deprecated `$screen-lg` as of v3.0.1
$screen-lg:                  1200px !default;
$screen-lg-min:              $screen-lg !default;
//** Deprecated `$screen-lg-desktop` as of v3.0.1
$screen-lg-desktop:          $screen-lg-min !default;

// So media queries don't overlap when required, provide a maximum
$screen-xs-max:              ($screen-sm-min - 1) !default;
$screen-sm-max:              ($screen-md-min - 1) !default;
$screen-md-max:              ($screen-lg-min - 1) !default;