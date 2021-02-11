# Advanced Markdown

## Abbreviations

The HTML specification is maintained by the W3C.

--8<-- "includes/abbreviations.md"

## Admonitions

!!! note
    You should note that the title will be automatically capitalized.

!!! danger "Attention"
    When executing below operation, the file will be permanently deleted.

    `remove-item 'test.txt'`

!!! tip "Top 5 electrical safety tips"
    - Replace or repair damaged power cords
    - Don't overload your outlets
    - Avoid extension cords as much as possible
    - Keep electrical equipment or outlets away from water
    - Protect small children from hazards

!!! warning ""
    It is always important to verify that a circuit is not live.

### Details

???+ note "Open styled details"

    ??? success
        This was great!

    ??? warning classes
        Please check the result.

## Buttons

Examples of links displayes as buttons.

[Subscribe to our mailing list](#){: .md-button }

[Connect with our sales team](#){: .md-button .md-button--primary }

[Submit :fontawesome-solid-paper-plane:](#){: .md-button }

## Code blocks

``` powershell
get-service |? { $_.Status -eq 'running' } | select -first 5
```

``` python linenums="1" hl_lines="10-13"
import turtle 
import math 
import colorsys 
 
phi = 180 * (3 - math.sqrt(5)) 
 
t = turtle.Pen() 
t.speed(0) 
 
def square(t, size): 
    for tmp in range(0,4): 
        t.forward(size) 
        t.right(90) 
  
num = 200 
 
for x in reversed(range(0, num)): 
    t.fillcolor(colorsys.hsv_to_rgb(x/num, 1.0, 1.0)) 
    t.begin_fill() 
    t.circle(5 + x, None, 11) 
    square(t, 5 + x) 
    t.end_fill() 
    t.right(phi) 
    t.right(.8) 
 
turtle.mainloop()
```
## Keys

Use the following combination to insert hyperlink without extra formatting:

++ctrl+shift+v++

## Content tabs

### Grouping code blocks

=== "C"

    ``` c
    #include <stdio.h>

    int main(void) {
      printf("Hello world!\n");
      return 0;
    }
    ```

=== "C++"

    ``` c++
    #include <iostream>

    int main(void) {
      std::cout << "Hello world!" << std::endl;
      return 0;
    }
    ```

### Grouping other content

??? example

    === "Unordered List"

        _Example_:

        ``` markdown
        * Sed sagittis eleifend rutrum
        * Donec vitae suscipit est
        * Nulla tempor lobortis orci
        ```

        _Result_:

        * Sed sagittis eleifend rutrum
        * Donec vitae suscipit est
        * Nulla tempor lobortis orci

    === "Ordered List"

        _Example_:

        ``` markdown
        1. Sed sagittis eleifend rutrum
        2. Donec vitae suscipit est
        3. Nulla tempor lobortis orci
        ```

        _Result_:

        1. Sed sagittis eleifend rutrum
        2. Donec vitae suscipit est
        3. Nulla tempor lobortis orci

## Tables

| Method      | Description                          |
| :---------- | :----------------------------------- |
| `GET`       | :material-check:     Fetch resource  |
| `PUT`       | :material-check-all: Update resource |
| `DELETE`    | :material-close:     Delete resource |

## Smart symbols

Examples of smart symbols supported:

- `c/o` - c/o
- `-->` - -->
- `=/=` - =/=
- `1/2` - 1/2
- `2nd` - 2nd

## Emoji

Ark is :chicken: :tractor:!

## Images

![Microsoft Team Assessment](https://images.squarespace-cdn.com/content/v1/5e6922809f4c330397d85090/1593457342989-MAE0DWX8MJ2VUVJT40UE/ke17ZwdGBToddI8pDm48kAt72yGFwHZjoxtmj75n0VMUqsxRUqqbr1mOJYKfIPR7LoDQ9mXPOjoJoqy81S2I8N_N4V1vUb5AoIIIbLZhVYy7Mythp_T-mtop-vrsUOmeInPi9iDjx9w8K4ZfjXt2dv608ZF5SQ066zrusfA3lZsto2GUPSkfCkjYhXQIm1t1CjLISwBs8eEdxAxTptZAUg/TeamsAssessment_Vee.png?format=300w){: align=right }

Monitor your Microsoft teams environment with this assessment. Teams is a powerful collaboration, file sharing, and communication platform, but you need to manage it effectively to get the most use.

## Definitions

`Lorem ipsum dolor sit amet`
:   Sed sagittis eleifend rutrum. Donec vitae suscipit est. Nullam tempus
    tellus non sem sollicitudin, quis rutrum leo facilisis.

`Cras arcu libero`
:   Aliquam metus eros, pretium sed nulla venenatis, faucibus auctor ex. Proin
    ut eros sed sapien ullamcorper consequat. Nunc ligula ante.

    Duis mollis est eget nibh volutpat, fermentum aliquet dui mollis.
    Nam vulputate tincidunt fringilla.
    Nullam dignissim ultrices urna non auctor.

## Task list

- [x] Lorem ipsum dolor sit amet, consectetur adipiscing elit
- [ ] Vestibulum convallis sit amet nisi a tincidunt
    * [x] In hac habitasse platea dictumst
    * [x] In scelerisque nibh non dolor mollis congue sed et metus
    * [ ] Praesent sed risus massa
- [ ] Aenean pretium efficitur erat, donec pharetra, ligula non scelerisque
