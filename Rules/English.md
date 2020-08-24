# Rules

Capture your opponent’s <span class="color-secundary">flag</span> with your <span class="color-secundary">robot</span> to win!

## 1. Setting up

Each player places his <span class="color-secundary">robot</span> on his <span class="color-secundary">start tile</span> and his <span class="color-secundary">flag</span> on <span class="color-secundary">base tile</span>. Then uses his <span class="color-secundary">barricade</span> to hide his <span class="color-secundary">buffer</span> from his opponent.

## 2. Turns

At the start of each turn, each player places his 3 <span class="color-secundary">commands</span> on his <span class="color-secundary">buffer</span>. There are 6 possible <span class="color-secundary">commands</span>:

* <span class="color-primary">Up</span>: Move your <span class="color-secundary">robot</span> one tile <span class="color-primary">upwards</span>
* <span class="color-primary">Down</span>: Move your <span class="color-secundary">robot</span> one tile <span class="color-primary">downwards</span>
* <span class="color-primary">Left</span>: Move your <span class="color-secundary">robot</span> one tile to the <span class="color-primary">left</span>
* <span class="color-primary">Right</span>: Move your <span class="color-secundary">robot</span> one tile to the <span class="color-primary">right</span>
* <span class="color-primary">Idle</span>: Your <span class="color-secundary">robot</span> don’t perform any action
* <span class="color-primary">Shoot</span>: Your <span class="color-secundary">robot</span> performs a <span class="color-primary">shot</span> affecting tiles in a cross pattern, like the tower range on chess. This includes all tiles <span class="color-primary">upwards</span>, <span class="color-primary">downwards</span>, <span class="color-primary">to the left</span> and <span class="color-primary">to the right</span>. If your opponent get caught it will be returned to the <span class="color-secundary">start tile</span>.

<span class="color-alert">Notice!</span> You can’t move to a wall, a tile occupied by an idle opponent or your <span class="color-secundary">flag</span> and to a tile that your opponent is also moving to. If you happen to do it, your <span class="color-secundary">robot</span> will bounce back to his tile of origin and the game will continue normally.

Once both are ready, they reveal their <span class="color-secundary">commands</span> at the same time, one by one in the respective order given by <span class="color-secundary">buffer</span>.

<span class="color-alert">Notice!</span> Movement <span class="color-secundary">commands</span> have priority over <span class="color-primary">shots</span>. This means every time you execute a pair of <span class="color-secundary">commands</span> (yours and your opponents) first execute movements (<span class="color-primary">up</span>, <span class="color-primary">down</span>, <span class="color-primary">left</span>, <span class="color-primary">right</span>) and then <span class="color-primary">shots</span> if any.

## 3. Winning the game

First capture your opponent's <span class="color-secundary">flag</span> by moving your <span class="color-secundary">robot</span> to the same tile as the <span class="color-secundary">flag</span>. Once captured, the <span class="color-secundary">flag</span> will move along your <span class="color-secundary">robot</span>. Win by bringing your opponent <span class="color-secundary">flag</span> back to your <span class="color-secundary">base tile</span> before your opponent!

## What if...

<span class="color-third">What if</span> both <span class="color-secundary">robots</span> bring the <span class="color-secundary">flag</span> back at the same time?

<span class="color-third">A/</span> That’s a tie! Play another round from the beginning to untie!

<span class="color-third">What if</span> you get <span class="color-primary">shot</span> while holding the <span class="color-secundary">flag</span>?

<span class="color-third">A/</span> Your <span class="color-secundary">robot</span> will drop the <span class="color-secundary">flag</span>! So your <span class="color-secundary">robot</span> gets back to the <span class="color-secundary">start tile</span> but the <span class="color-secundary">flag</span> stays on the square where the robot was <span class="color-primary">shot</span>.

<span class="color-third">What if</span> you get <span class="color-primary">shot</span> but still have <span class="color-secundary">commands</span> left on the <span class="color-secundary">buffer</span>?

<span class="color-third">A/</span> Continue executing them normally! But relatively to the new <span class="color-secundary">robot</span> position.

<span class="color-third">What if</span> you get <span class="color-primary">shot</span> and your start tile is occupied by either your opponent or your <span class="color-secundary">flag</span>?

<span class="color-third">A/</span> In this specific case your opponent wins! You can’t share the same square with your opponent or <span class="color-secundary">flag</span> so be careful!

## Glossary

* <span class="color-secundary">Robot</span>: Playable character. Outbuffered is a 2 player game and each player controls a <span class="color-secundary">robot</span> of his own. <img src="../PNG/renders/robo.png" height="50"/>
* <span class="color-secundary">Flag</span>: Each player has a <span class="color-secundary">flag</span>, your objective is to bring your opponent’s <span class="color-secundary">flag</span> to your <span class="color-secundary">base tile</span>. <img src="../PNG/renders/flag.png" height="50"/>
* <span class="color-secundary">Base tile</span>: Tile where your <span class="color-secundary">flag</span> is located at the beginning of the match and where you bring your opponent's <span class="color-secundary">flag</span> to win.
* <span class="color-secundary">Start tile</span>: Special tile where <span class="color-secundary">robots</span> are located at the beginning of each match.
* <span class="color-secundary">Command</span>: Action that your <span class="color-secundary">robot</span> will execute. In order to execute a <span class="color-secundary">command</span>, properly place it face up on your <span class="color-secundary">buffer</span>. <img src="../PNG/renders/command2.png" height="50"/>
* <span class="color-secundary">Buffer</span>: Command holder, each turn you choose the <span class="color-secundary">commands</span> and place them on your  <span class="color-secundary">buffer</span> in the corresponding order from first to last. <img src="../PNG/renders/buffer.png" height="50"/>
* <span class="color-secundary">Barricade</span>: Barrier used to prevent your opponent from peeking at your <span class="color-secundary">buffer</span>. <img src="../PNG/renders/barricade.png" height="50"/>

<style>
.color-primary{
  color: #c1d82fff;
}
.color-secundary{
  color: #aa54d2ff;
}
.color-third{
  color: #00c3c8ff;
}
.color-alert{
  color: #e70029ff;
}
</style>