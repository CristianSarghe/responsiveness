
# SCSS Responsiveness Helper


### What's in the repo?

* A ready-to-use SCSS file with mixins to help handling **web page responsiveness**

### Usage

1. Download the file (or copy the contents)
2. Please keep the creator's references in the file
3. Modify breakpoint values if needed
4. Use mixins wherever needed to add SCSS according to the preset breakpoints

### Mentions

* **Breakpoints** (although named `sm`, `md`, `lg`, `xl`) represent a single number which is considered the *lower boundary* of the interval they borrow name from.
* **Mixins** `media-xs`, `media-sm`, `media-md`, `media-lg`, `media-xl` refer to an *interval* 
* The mixin names are self-explanatory

### Example

     @import "responsiveness";
     
     button {
        @include media-below($breakpoint-sm) {
          color: red;
        }
        
        @include media-sm {
          color: green;
        }
        
        @include media-above($breakpoint-md) {
          color: blue;
        }
     }

