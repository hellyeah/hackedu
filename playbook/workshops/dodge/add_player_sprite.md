# Adding the Player Sprite

Currently our canvas is blank like this:

![](img/sq_1_blank_canvas.png)

We want to eventually make the player sprite look like this:

![](img/sq_5_player_image.gif)

But for now, we'll settle with this:

![](img/sq_2_add_player_sprite.png)

## Adding the Player Sprite

We can add the plyaer sprite with the following code (new code highlited in
purple)

> [![](img/2_js_bin_screenshot.png)](http://jsbin.com/qiyuno/14/edit?js,output)

[![](img/open_in_js_bin.png)](http://jsbin.com/qiyuno/14/edit?js,output)

The highlighted purple lines above (reproduced below) are responsible for adding
the player sprite.

## Tinkering with the values of `createSprite`

![](img/checkmark.png) Open [the above JS Bin](http://jsbin.com/qiyuno/14/edit?js,output) and try messing around with the starting position of the sprite.

Here is an example of how I play around with the values of `createSprite` to try
to understand what it does:

> ![](img/2_messing_around_with_starting_position.gif)

## Understanding `createSprite`

There are 3 parts to creating a sprite:

1. creating a variable to store the sprite in
2. creating the actual sprite and storing it in the above variable
3. drawing the sprite

1. First we need to create the variable `player` to store the sprite in:

> ![](img/2_variable.png)

2. Then we actually create the sprite and store it in the variable `player`:

> ![](img/2_create_sprite.png)

```
player = createSprite(150, 450);
  ^                    ^    ^
  |                    |    └ set the *y* coordinate of the sprite
  |                    |
  |                    └ set the *x* coordinate of the sprite
  └ Store the newly
    created sprite
    with the variable `player`
```

> ![](img/t2_sprite_position.png)

3. Then we have to tell the program to actually draw the sprites in our program
by calling `drawSprites()`:

> ![](img/2_draw_sprites.png)

If we don't include `drawSprites()`, even if the sprites have been created, you
cannot see them.

## Adding the Sprite to Your Code

![](img/checkmark.png) Now add the 3 lines of code needed to add the sprite to
your "_**working bin**_".

> ![](img/t2_add_code.gif)

## Recap

We learned how to:

- create a variable
- create a new sprite with `createSprite`
- the new sprite's starting position
- store a sprite into a variable
- draw the sprite

## Next Up

| **[![](img/sq_3_linear_player_movement.gif)  <br> 3. Linear Player Movement] (linear_player_movement.md)**    |
|:--------------------------------------------------------------------------------------------------------------|

--------------------------------------------------------------------------------

<!--

Commented this out because it's not good enough yet.

I want to leave it in the comments because it has some work done on it

## Appendix

### Documentation ![](img/documentation.png)

#### [p5.js Play Documentation](http://p5play.molleindustria.org/docs/index.html)

- [`createSprite(150, 450)`]
(http://p5play.molleindustria.org/docs/classes/p5.play.html#method-createSprite)

#### Understanding the Computer Science Fundamentals ![](img/computer_science.png)

```
This section goes over some of the fundamental programming concepts, you can
feel free to skip this section if you like.
```

In order for a program to remember something, we must use a variable to remember
it. And so we create the `player` variable to remember the player sprite.

> ![](img/2_variable.png)

`createSprite is a function` functions have 3 components

- inputs
- actions
- output

... -->

## Table of Contents

| **[![](img/sq_1_blank_canvas.png)          <br> 1.  Blank Canvas]      (blank_canvas.md)**          | **[![](img/sq_2_add_player_sprite.png)    <br> 2. Add Player Sprite]    (add_player_sprite.md)**    | **[![](img/sq_3_linear_player_movement.gif)  <br> 3. Linear Player Movement] (linear_player_movement.md)** |
|:----------------------------------------------------------------------------------------------------|:----------------------------------------------------------------------------------------------------|:-----------------------------------------------------------------------------------------------------------|
| **[![](img/sq_4_arrow_key_movement.gif)    <br> 4.  Arrow Key Movement](arrow_key_movement.md)**    | **[![](img/sq_5_player_image.gif)         <br> 5. Player Image]         (player_image.md)**         | **[![](img/sq_6_add_enemy_sprite.gif)        <br> 6. Add Enemy Sprite]       (add_enemy_sprite.md)**       |
| **[![](img/sq_7_linear_enemy_movement.gif) <br> 7.  Enemy Sprite Move] (linear_enemy_movement.md)** | **[![](img/sq_8_enemy_go_back_to_top.gif) <br> 8. Enemy Go Back to Top] (enemy_go_back_to_top.md)** | **[![](img/sq_9_random_enemy_position.gif)   <br> 9. Random Enemy Position]  (random_enemy_position.md)**  |
| **[![](img/sq_10_game_over.gif)            <br> 10. Game Over]         (game_over.md)**             |                                                                                                     | **[![](img/readme.png) <br> Back to the README.md](README.md)**                                            |