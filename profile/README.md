# Tic-Tac-Toe (playable right here)

No JavaScript, no build, no leaving the page. GitHub strips `<script>` from
rendered markdown, so this game runs on the one interactive primitive that
survives sanitization: nested `<details>` elements.

Every legal line of play is precomputed. You are **X** and move first. **O** is
a minimax agent that never loses — the best you can do is force a draw.

**How to play:** expand the move you want. O's reply appears immediately, along
with the board and your next set of choices. To take a move back, collapse that
section and expand a different one.

The board labels empty squares with their number:

<pre>
 1 | 2 | 3
---+---+---
 4 | 5 | 6
---+---+---
 7 | 8 | 9
</pre>

---

## Your move

<details><summary>Play X at 1</summary><pre>
 X | 2 | 3
---+---+---
 4 | O | 6
---+---+---
 7 | 8 | 9
</pre>
O responds at 5. Your move:
<details><summary>Play X at 2</summary><pre>
 X | X | O
---+---+---
 4 | O | 6
---+---+---
 7 | 8 | 9
</pre>
O responds at 3. Your move:
<details><summary>Play X at 4</summary><pre>
 X | X | O
---+---+---
 X | O | 6
---+---+---
 O | 8 | 9
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 6</summary><pre>
 X | X | O
---+---+---
 4 | O | X
---+---+---
 O | 8 | 9
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 7</summary><pre>
 X | X | O
---+---+---
 O | O | 6
---+---+---
 X | 8 | 9
</pre>
O responds at 4. Your move:
<details><summary>Play X at 6</summary><pre>
 X | X | O
---+---+---
 O | O | X
---+---+---
 X | O | 9
</pre>
O responds at 8. Your move:
<details><summary>Play X at 9</summary><pre>
 X | X | O
---+---+---
 O | O | X
---+---+---
 X | O | X
</pre><b>Draw. Best possible result against a perfect opponent.</b>
</details>
</details>
<details><summary>Play X at 8</summary><pre>
 X | X | O
---+---+---
 O | O | O
---+---+---
 X | X | 9
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 9</summary><pre>
 X | X | O
---+---+---
 O | O | O
---+---+---
 X | 8 | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
</details>
<details><summary>Play X at 8</summary><pre>
 X | X | O
---+---+---
 O | O | 6
---+---+---
 7 | X | 9
</pre>
O responds at 4. Your move:
<details><summary>Play X at 6</summary><pre>
 X | X | O
---+---+---
 O | O | X
---+---+---
 O | X | 9
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 7</summary><pre>
 X | X | O
---+---+---
 O | O | O
---+---+---
 X | X | 9
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 9</summary><pre>
 X | X | O
---+---+---
 O | O | O
---+---+---
 7 | X | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
</details>
<details><summary>Play X at 9</summary><pre>
 X | X | O
---+---+---
 O | O | 6
---+---+---
 7 | 8 | X
</pre>
O responds at 4. Your move:
<details><summary>Play X at 6</summary><pre>
 X | X | O
---+---+---
 O | O | X
---+---+---
 O | 8 | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 7</summary><pre>
 X | X | O
---+---+---
 O | O | O
---+---+---
 X | 8 | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 8</summary><pre>
 X | X | O
---+---+---
 O | O | O
---+---+---
 7 | X | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
</details>
</details>
<details><summary>Play X at 3</summary><pre>
 X | O | X
---+---+---
 4 | O | 6
---+---+---
 7 | 8 | 9
</pre>
O responds at 2. Your move:
<details><summary>Play X at 4</summary><pre>
 X | O | X
---+---+---
 X | O | 6
---+---+---
 7 | O | 9
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 6</summary><pre>
 X | O | X
---+---+---
 4 | O | X
---+---+---
 7 | O | 9
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 7</summary><pre>
 X | O | X
---+---+---
 O | O | 6
---+---+---
 X | 8 | 9
</pre>
O responds at 4. Your move:
<details><summary>Play X at 6</summary><pre>
 X | O | X
---+---+---
 O | O | X
---+---+---
 X | O | 9
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 8</summary><pre>
 X | O | X
---+---+---
 O | O | O
---+---+---
 X | X | 9
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 9</summary><pre>
 X | O | X
---+---+---
 O | O | O
---+---+---
 X | 8 | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
</details>
<details><summary>Play X at 8</summary><pre>
 X | O | X
---+---+---
 O | O | 6
---+---+---
 7 | X | 9
</pre>
O responds at 4. Your move:
<details><summary>Play X at 6</summary><pre>
 X | O | X
---+---+---
 O | O | X
---+---+---
 7 | X | O
</pre>
O responds at 9. Your move:
<details><summary>Play X at 7</summary><pre>
 X | O | X
---+---+---
 O | O | X
---+---+---
 X | X | O
</pre><b>Draw. Best possible result against a perfect opponent.</b>
</details>
</details>
<details><summary>Play X at 7</summary><pre>
 X | O | X
---+---+---
 O | O | O
---+---+---
 X | X | 9
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 9</summary><pre>
 X | O | X
---+---+---
 O | O | O
---+---+---
 7 | X | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
</details>
<details><summary>Play X at 9</summary><pre>
 X | O | X
---+---+---
 4 | O | O
---+---+---
 7 | 8 | X
</pre>
O responds at 6. Your move:
<details><summary>Play X at 4</summary><pre>
 X | O | X
---+---+---
 X | O | O
---+---+---
 7 | O | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 7</summary><pre>
 X | O | X
---+---+---
 O | O | O
---+---+---
 X | 8 | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 8</summary><pre>
 X | O | X
---+---+---
 O | O | O
---+---+---
 7 | X | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
</details>
</details>
<details><summary>Play X at 4</summary><pre>
 X | 2 | 3
---+---+---
 X | O | 6
---+---+---
 O | 8 | 9
</pre>
O responds at 7. Your move:
<details><summary>Play X at 2</summary><pre>
 X | X | O
---+---+---
 X | O | 6
---+---+---
 O | 8 | 9
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 3</summary><pre>
 X | O | X
---+---+---
 X | O | 6
---+---+---
 O | 8 | 9
</pre>
O responds at 2. Your move:
<details><summary>Play X at 6</summary><pre>
 X | O | X
---+---+---
 X | O | X
---+---+---
 O | O | 9
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 8</summary><pre>
 X | O | X
---+---+---
 X | O | O
---+---+---
 O | X | 9
</pre>
O responds at 6. Your move:
<details><summary>Play X at 9</summary><pre>
 X | O | X
---+---+---
 X | O | O
---+---+---
 O | X | X
</pre><b>Draw. Best possible result against a perfect opponent.</b>
</details>
</details>
<details><summary>Play X at 9</summary><pre>
 X | O | X
---+---+---
 X | O | 6
---+---+---
 O | O | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
</details>
<details><summary>Play X at 6</summary><pre>
 X | O | 3
---+---+---
 X | O | X
---+---+---
 O | 8 | 9
</pre>
O responds at 2. Your move:
<details><summary>Play X at 3</summary><pre>
 X | O | X
---+---+---
 X | O | X
---+---+---
 O | O | 9
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 8</summary><pre>
 X | O | O
---+---+---
 X | O | X
---+---+---
 O | X | 9
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 9</summary><pre>
 X | O | O
---+---+---
 X | O | X
---+---+---
 O | 8 | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
</details>
<details><summary>Play X at 8</summary><pre>
 X | 2 | O
---+---+---
 X | O | 6
---+---+---
 O | X | 9
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 9</summary><pre>
 X | O | 3
---+---+---
 X | O | 6
---+---+---
 O | 8 | X
</pre>
O responds at 2. Your move:
<details><summary>Play X at 3</summary><pre>
 X | O | X
---+---+---
 X | O | 6
---+---+---
 O | O | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 6</summary><pre>
 X | O | O
---+---+---
 X | O | X
---+---+---
 O | 8 | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 8</summary><pre>
 X | O | O
---+---+---
 X | O | 6
---+---+---
 O | X | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
</details>
</details>
<details><summary>Play X at 6</summary><pre>
 X | O | 3
---+---+---
 4 | O | X
---+---+---
 7 | 8 | 9
</pre>
O responds at 2. Your move:
<details><summary>Play X at 3</summary><pre>
 X | O | X
---+---+---
 4 | O | X
---+---+---
 7 | O | 9
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 4</summary><pre>
 X | O | 3
---+---+---
 X | O | X
---+---+---
 O | 8 | 9
</pre>
O responds at 7. Your move:
<details><summary>Play X at 3</summary><pre>
 X | O | X
---+---+---
 X | O | X
---+---+---
 O | O | 9
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 8</summary><pre>
 X | O | O
---+---+---
 X | O | X
---+---+---
 O | X | 9
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 9</summary><pre>
 X | O | O
---+---+---
 X | O | X
---+---+---
 O | 8 | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
</details>
<details><summary>Play X at 7</summary><pre>
 X | O | 3
---+---+---
 4 | O | X
---+---+---
 X | O | 9
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 8</summary><pre>
 X | O | 3
---+---+---
 4 | O | X
---+---+---
 O | X | 9
</pre>
O responds at 7. Your move:
<details><summary>Play X at 3</summary><pre>
 X | O | X
---+---+---
 4 | O | X
---+---+---
 O | X | O
</pre>
O responds at 9. Your move:
<details><summary>Play X at 4</summary><pre>
 X | O | X
---+---+---
 X | O | X
---+---+---
 O | X | O
</pre><b>Draw. Best possible result against a perfect opponent.</b>
</details>
</details>
<details><summary>Play X at 4</summary><pre>
 X | O | O
---+---+---
 X | O | X
---+---+---
 O | X | 9
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 9</summary><pre>
 X | O | O
---+---+---
 4 | O | X
---+---+---
 O | X | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
</details>
<details><summary>Play X at 9</summary><pre>
 X | O | O
---+---+---
 4 | O | X
---+---+---
 7 | 8 | X
</pre>
O responds at 3. Your move:
<details><summary>Play X at 4</summary><pre>
 X | O | O
---+---+---
 X | O | X
---+---+---
 O | 8 | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 7</summary><pre>
 X | O | O
---+---+---
 4 | O | X
---+---+---
 X | O | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 8</summary><pre>
 X | O | O
---+---+---
 4 | O | X
---+---+---
 O | X | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
</details>
</details>
<details><summary>Play X at 7</summary><pre>
 X | 2 | 3
---+---+---
 O | O | 6
---+---+---
 X | 8 | 9
</pre>
O responds at 4. Your move:
<details><summary>Play X at 2</summary><pre>
 X | X | 3
---+---+---
 O | O | O
---+---+---
 X | 8 | 9
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 3</summary><pre>
 X | O | X
---+---+---
 O | O | 6
---+---+---
 X | 8 | 9
</pre>
O responds at 2. Your move:
<details><summary>Play X at 6</summary><pre>
 X | O | X
---+---+---
 O | O | X
---+---+---
 X | O | 9
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 8</summary><pre>
 X | O | X
---+---+---
 O | O | O
---+---+---
 X | X | 9
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 9</summary><pre>
 X | O | X
---+---+---
 O | O | O
---+---+---
 X | 8 | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
</details>
<details><summary>Play X at 6</summary><pre>
 X | O | 3
---+---+---
 O | O | X
---+---+---
 X | 8 | 9
</pre>
O responds at 2. Your move:
<details><summary>Play X at 3</summary><pre>
 X | O | X
---+---+---
 O | O | X
---+---+---
 X | O | 9
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 8</summary><pre>
 X | O | 3
---+---+---
 O | O | X
---+---+---
 X | X | O
</pre>
O responds at 9. Your move:
<details><summary>Play X at 3</summary><pre>
 X | O | X
---+---+---
 O | O | X
---+---+---
 X | X | O
</pre><b>Draw. Best possible result against a perfect opponent.</b>
</details>
</details>
<details><summary>Play X at 9</summary><pre>
 X | O | 3
---+---+---
 O | O | X
---+---+---
 X | O | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
</details>
<details><summary>Play X at 8</summary><pre>
 X | 2 | 3
---+---+---
 O | O | O
---+---+---
 X | X | 9
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 9</summary><pre>
 X | 2 | 3
---+---+---
 O | O | O
---+---+---
 X | 8 | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
</details>
<details><summary>Play X at 8</summary><pre>
 X | 2 | 3
---+---+---
 O | O | 6
---+---+---
 7 | X | 9
</pre>
O responds at 4. Your move:
<details><summary>Play X at 2</summary><pre>
 X | X | O
---+---+---
 O | O | 6
---+---+---
 7 | X | 9
</pre>
O responds at 3. Your move:
<details><summary>Play X at 6</summary><pre>
 X | X | O
---+---+---
 O | O | X
---+---+---
 O | X | 9
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 7</summary><pre>
 X | X | O
---+---+---
 O | O | O
---+---+---
 X | X | 9
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 9</summary><pre>
 X | X | O
---+---+---
 O | O | O
---+---+---
 7 | X | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
</details>
<details><summary>Play X at 3</summary><pre>
 X | 2 | X
---+---+---
 O | O | O
---+---+---
 7 | X | 9
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 6</summary><pre>
 X | 2 | O
---+---+---
 O | O | X
---+---+---
 7 | X | 9
</pre>
O responds at 3. Your move:
<details><summary>Play X at 2</summary><pre>
 X | X | O
---+---+---
 O | O | X
---+---+---
 O | X | 9
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 7</summary><pre>
 X | 2 | O
---+---+---
 O | O | X
---+---+---
 X | X | O
</pre>
O responds at 9. Your move:
<details><summary>Play X at 2</summary><pre>
 X | X | O
---+---+---
 O | O | X
---+---+---
 X | X | O
</pre><b>Draw. Best possible result against a perfect opponent.</b>
</details>
</details>
<details><summary>Play X at 9</summary><pre>
 X | 2 | O
---+---+---
 O | O | X
---+---+---
 O | X | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
</details>
<details><summary>Play X at 7</summary><pre>
 X | 2 | 3
---+---+---
 O | O | O
---+---+---
 X | X | 9
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 9</summary><pre>
 X | 2 | 3
---+---+---
 O | O | O
---+---+---
 7 | X | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
</details>
<details><summary>Play X at 9</summary><pre>
 X | O | 3
---+---+---
 4 | O | 6
---+---+---
 7 | 8 | X
</pre>
O responds at 2. Your move:
<details><summary>Play X at 3</summary><pre>
 X | O | X
---+---+---
 4 | O | O
---+---+---
 7 | 8 | X
</pre>
O responds at 6. Your move:
<details><summary>Play X at 4</summary><pre>
 X | O | X
---+---+---
 X | O | O
---+---+---
 7 | O | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 7</summary><pre>
 X | O | X
---+---+---
 O | O | O
---+---+---
 X | 8 | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 8</summary><pre>
 X | O | X
---+---+---
 O | O | O
---+---+---
 7 | X | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
</details>
<details><summary>Play X at 4</summary><pre>
 X | O | 3
---+---+---
 X | O | 6
---+---+---
 O | 8 | X
</pre>
O responds at 7. Your move:
<details><summary>Play X at 3</summary><pre>
 X | O | X
---+---+---
 X | O | 6
---+---+---
 O | O | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 6</summary><pre>
 X | O | O
---+---+---
 X | O | X
---+---+---
 O | 8 | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 8</summary><pre>
 X | O | O
---+---+---
 X | O | 6
---+---+---
 O | X | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
</details>
<details><summary>Play X at 6</summary><pre>
 X | O | O
---+---+---
 4 | O | X
---+---+---
 7 | 8 | X
</pre>
O responds at 3. Your move:
<details><summary>Play X at 4</summary><pre>
 X | O | O
---+---+---
 X | O | X
---+---+---
 O | 8 | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 7</summary><pre>
 X | O | O
---+---+---
 4 | O | X
---+---+---
 X | O | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 8</summary><pre>
 X | O | O
---+---+---
 4 | O | X
---+---+---
 O | X | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
</details>
<details><summary>Play X at 7</summary><pre>
 X | O | 3
---+---+---
 4 | O | 6
---+---+---
 X | O | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 8</summary><pre>
 X | O | 3
---+---+---
 4 | O | 6
---+---+---
 O | X | X
</pre>
O responds at 7. Your move:
<details><summary>Play X at 3</summary><pre>
 X | O | X
---+---+---
 4 | O | O
---+---+---
 O | X | X
</pre>
O responds at 6. Your move:
<details><summary>Play X at 4</summary><pre>
 X | O | X
---+---+---
 X | O | O
---+---+---
 O | X | X
</pre><b>Draw. Best possible result against a perfect opponent.</b>
</details>
</details>
<details><summary>Play X at 4</summary><pre>
 X | O | O
---+---+---
 X | O | 6
---+---+---
 O | X | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 6</summary><pre>
 X | O | O
---+---+---
 4 | O | X
---+---+---
 O | X | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
</details>
</details>
</details>
<details><summary>Play X at 2</summary><pre>
 O | X | 3
---+---+---
 4 | 5 | 6
---+---+---
 7 | 8 | 9
</pre>
O responds at 1. Your move:
<details><summary>Play X at 3</summary><pre>
 O | X | X
---+---+---
 O | 5 | 6
---+---+---
 7 | 8 | 9
</pre>
O responds at 4. Your move:
<details><summary>Play X at 5</summary><pre>
 O | X | X
---+---+---
 O | X | 6
---+---+---
 O | 8 | 9
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 6</summary><pre>
 O | X | X
---+---+---
 O | 5 | X
---+---+---
 O | 8 | 9
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 7</summary><pre>
 O | X | X
---+---+---
 O | O | 6
---+---+---
 X | 8 | 9
</pre>
O responds at 5. Your move:
<details><summary>Play X at 6</summary><pre>
 O | X | X
---+---+---
 O | O | X
---+---+---
 X | 8 | O
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 8</summary><pre>
 O | X | X
---+---+---
 O | O | O
---+---+---
 X | X | 9
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 9</summary><pre>
 O | X | X
---+---+---
 O | O | O
---+---+---
 X | 8 | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
</details>
<details><summary>Play X at 8</summary><pre>
 O | X | X
---+---+---
 O | O | 6
---+---+---
 7 | X | 9
</pre>
O responds at 5. Your move:
<details><summary>Play X at 6</summary><pre>
 O | X | X
---+---+---
 O | O | X
---+---+---
 O | X | 9
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 7</summary><pre>
 O | X | X
---+---+---
 O | O | O
---+---+---
 X | X | 9
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 9</summary><pre>
 O | X | X
---+---+---
 O | O | O
---+---+---
 7 | X | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
</details>
<details><summary>Play X at 9</summary><pre>
 O | X | X
---+---+---
 O | 5 | O
---+---+---
 7 | 8 | X
</pre>
O responds at 6. Your move:
<details><summary>Play X at 5</summary><pre>
 O | X | X
---+---+---
 O | X | O
---+---+---
 O | 8 | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 7</summary><pre>
 O | X | X
---+---+---
 O | O | O
---+---+---
 X | 8 | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 8</summary><pre>
 O | X | X
---+---+---
 O | O | O
---+---+---
 7 | X | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
</details>
</details>
<details><summary>Play X at 4</summary><pre>
 O | X | 3
---+---+---
 X | O | 6
---+---+---
 7 | 8 | 9
</pre>
O responds at 5. Your move:
<details><summary>Play X at 3</summary><pre>
 O | X | X
---+---+---
 X | O | 6
---+---+---
 7 | 8 | O
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 6</summary><pre>
 O | X | O
---+---+---
 X | O | X
---+---+---
 7 | 8 | 9
</pre>
O responds at 3. Your move:
<details><summary>Play X at 7</summary><pre>
 O | X | O
---+---+---
 X | O | X
---+---+---
 X | 8 | O
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 8</summary><pre>
 O | X | O
---+---+---
 X | O | X
---+---+---
 O | X | 9
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 9</summary><pre>
 O | X | O
---+---+---
 X | O | X
---+---+---
 O | 8 | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
</details>
<details><summary>Play X at 7</summary><pre>
 O | X | 3
---+---+---
 X | O | 6
---+---+---
 X | 8 | O
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 8</summary><pre>
 O | X | O
---+---+---
 X | O | 6
---+---+---
 7 | X | 9
</pre>
O responds at 3. Your move:
<details><summary>Play X at 6</summary><pre>
 O | X | O
---+---+---
 X | O | X
---+---+---
 O | X | 9
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 7</summary><pre>
 O | X | O
---+---+---
 X | O | 6
---+---+---
 X | X | O
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 9</summary><pre>
 O | X | O
---+---+---
 X | O | 6
---+---+---
 O | X | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
</details>
<details><summary>Play X at 9</summary><pre>
 O | X | O
---+---+---
 X | O | 6
---+---+---
 7 | 8 | X
</pre>
O responds at 3. Your move:
<details><summary>Play X at 6</summary><pre>
 O | X | O
---+---+---
 X | O | X
---+---+---
 O | 8 | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 7</summary><pre>
 O | X | O
---+---+---
 X | O | 6
---+---+---
 X | O | X
</pre>
O responds at 8. Your move:
<details><summary>Play X at 6</summary><pre>
 O | X | O
---+---+---
 X | O | X
---+---+---
 X | O | X
</pre><b>Draw. Best possible result against a perfect opponent.</b>
</details>
</details>
<details><summary>Play X at 8</summary><pre>
 O | X | O
---+---+---
 X | O | 6
---+---+---
 O | X | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
</details>
</details>
<details><summary>Play X at 5</summary><pre>
 O | X | 3
---+---+---
 4 | X | 6
---+---+---
 7 | O | 9
</pre>
O responds at 8. Your move:
<details><summary>Play X at 3</summary><pre>
 O | X | X
---+---+---
 4 | X | 6
---+---+---
 O | O | 9
</pre>
O responds at 7. Your move:
<details><summary>Play X at 4</summary><pre>
 O | X | X
---+---+---
 X | X | 6
---+---+---
 O | O | O
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 6</summary><pre>
 O | X | X
---+---+---
 O | X | X
---+---+---
 O | O | 9
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 9</summary><pre>
 O | X | X
---+---+---
 O | X | 6
---+---+---
 O | O | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
</details>
<details><summary>Play X at 4</summary><pre>
 O | X | 3
---+---+---
 X | X | O
---+---+---
 7 | O | 9
</pre>
O responds at 6. Your move:
<details><summary>Play X at 3</summary><pre>
 O | X | X
---+---+---
 X | X | O
---+---+---
 O | O | 9
</pre>
O responds at 7. Your move:
<details><summary>Play X at 9</summary><pre>
 O | X | X
---+---+---
 X | X | O
---+---+---
 O | O | X
</pre><b>Draw. Best possible result against a perfect opponent.</b>
</details>
</details>
<details><summary>Play X at 7</summary><pre>
 O | X | O
---+---+---
 X | X | O
---+---+---
 X | O | 9
</pre>
O responds at 3. Your move:
<details><summary>Play X at 9</summary><pre>
 O | X | O
---+---+---
 X | X | O
---+---+---
 X | O | X
</pre><b>Draw. Best possible result against a perfect opponent.</b>
</details>
</details>
<details><summary>Play X at 9</summary><pre>
 O | X | O
---+---+---
 X | X | O
---+---+---
 7 | O | X
</pre>
O responds at 3. Your move:
<details><summary>Play X at 7</summary><pre>
 O | X | O
---+---+---
 X | X | O
---+---+---
 X | O | X
</pre><b>Draw. Best possible result against a perfect opponent.</b>
</details>
</details>
</details>
<details><summary>Play X at 6</summary><pre>
 O | X | 3
---+---+---
 O | X | X
---+---+---
 7 | O | 9
</pre>
O responds at 4. Your move:
<details><summary>Play X at 3</summary><pre>
 O | X | X
---+---+---
 O | X | X
---+---+---
 O | O | 9
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 7</summary><pre>
 O | X | O
---+---+---
 O | X | X
---+---+---
 X | O | 9
</pre>
O responds at 3. Your move:
<details><summary>Play X at 9</summary><pre>
 O | X | O
---+---+---
 O | X | X
---+---+---
 X | O | X
</pre><b>Draw. Best possible result against a perfect opponent.</b>
</details>
</details>
<details><summary>Play X at 9</summary><pre>
 O | X | 3
---+---+---
 O | X | X
---+---+---
 O | O | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
</details>
<details><summary>Play X at 7</summary><pre>
 O | X | O
---+---+---
 4 | X | 6
---+---+---
 X | O | 9
</pre>
O responds at 3. Your move:
<details><summary>Play X at 4</summary><pre>
 O | X | O
---+---+---
 X | X | O
---+---+---
 X | O | 9
</pre>
O responds at 6. Your move:
<details><summary>Play X at 9</summary><pre>
 O | X | O
---+---+---
 X | X | O
---+---+---
 X | O | X
</pre><b>Draw. Best possible result against a perfect opponent.</b>
</details>
</details>
<details><summary>Play X at 6</summary><pre>
 O | X | O
---+---+---
 O | X | X
---+---+---
 X | O | 9
</pre>
O responds at 4. Your move:
<details><summary>Play X at 9</summary><pre>
 O | X | O
---+---+---
 O | X | X
---+---+---
 X | O | X
</pre><b>Draw. Best possible result against a perfect opponent.</b>
</details>
</details>
<details><summary>Play X at 9</summary><pre>
 O | X | O
---+---+---
 O | X | 6
---+---+---
 X | O | X
</pre>
O responds at 4. Your move:
<details><summary>Play X at 6</summary><pre>
 O | X | O
---+---+---
 O | X | X
---+---+---
 X | O | X
</pre><b>Draw. Best possible result against a perfect opponent.</b>
</details>
</details>
</details>
<details><summary>Play X at 9</summary><pre>
 O | X | O
---+---+---
 4 | X | 6
---+---+---
 7 | O | X
</pre>
O responds at 3. Your move:
<details><summary>Play X at 4</summary><pre>
 O | X | O
---+---+---
 X | X | O
---+---+---
 7 | O | X
</pre>
O responds at 6. Your move:
<details><summary>Play X at 7</summary><pre>
 O | X | O
---+---+---
 X | X | O
---+---+---
 X | O | X
</pre><b>Draw. Best possible result against a perfect opponent.</b>
</details>
</details>
<details><summary>Play X at 6</summary><pre>
 O | X | O
---+---+---
 O | X | X
---+---+---
 7 | O | X
</pre>
O responds at 4. Your move:
<details><summary>Play X at 7</summary><pre>
 O | X | O
---+---+---
 O | X | X
---+---+---
 X | O | X
</pre><b>Draw. Best possible result against a perfect opponent.</b>
</details>
</details>
<details><summary>Play X at 7</summary><pre>
 O | X | O
---+---+---
 O | X | 6
---+---+---
 X | O | X
</pre>
O responds at 4. Your move:
<details><summary>Play X at 6</summary><pre>
 O | X | O
---+---+---
 O | X | X
---+---+---
 X | O | X
</pre><b>Draw. Best possible result against a perfect opponent.</b>
</details>
</details>
</details>
</details>
<details><summary>Play X at 6</summary><pre>
 O | X | 3
---+---+---
 4 | 5 | X
---+---+---
 O | 8 | 9
</pre>
O responds at 7. Your move:
<details><summary>Play X at 3</summary><pre>
 O | X | X
---+---+---
 O | 5 | X
---+---+---
 O | 8 | 9
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 4</summary><pre>
 O | X | 3
---+---+---
 X | O | X
---+---+---
 O | 8 | 9
</pre>
O responds at 5. Your move:
<details><summary>Play X at 3</summary><pre>
 O | X | X
---+---+---
 X | O | X
---+---+---
 O | 8 | O
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 8</summary><pre>
 O | X | O
---+---+---
 X | O | X
---+---+---
 O | X | 9
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 9</summary><pre>
 O | X | O
---+---+---
 X | O | X
---+---+---
 O | 8 | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
</details>
<details><summary>Play X at 5</summary><pre>
 O | X | 3
---+---+---
 O | X | X
---+---+---
 O | 8 | 9
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 8</summary><pre>
 O | X | 3
---+---+---
 O | 5 | X
---+---+---
 O | X | 9
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 9</summary><pre>
 O | X | O
---+---+---
 4 | 5 | X
---+---+---
 O | 8 | X
</pre>
O responds at 3. Your move:
<details><summary>Play X at 4</summary><pre>
 O | X | O
---+---+---
 X | O | X
---+---+---
 O | 8 | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 5</summary><pre>
 O | X | O
---+---+---
 O | X | X
---+---+---
 O | 8 | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 8</summary><pre>
 O | X | O
---+---+---
 O | 5 | X
---+---+---
 O | X | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
</details>
</details>
<details><summary>Play X at 7</summary><pre>
 O | X | 3
---+---+---
 4 | O | 6
---+---+---
 X | 8 | 9
</pre>
O responds at 5. Your move:
<details><summary>Play X at 3</summary><pre>
 O | X | X
---+---+---
 O | O | 6
---+---+---
 X | 8 | 9
</pre>
O responds at 4. Your move:
<details><summary>Play X at 6</summary><pre>
 O | X | X
---+---+---
 O | O | X
---+---+---
 X | 8 | O
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 8</summary><pre>
 O | X | X
---+---+---
 O | O | O
---+---+---
 X | X | 9
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 9</summary><pre>
 O | X | X
---+---+---
 O | O | O
---+---+---
 X | 8 | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
</details>
<details><summary>Play X at 4</summary><pre>
 O | X | 3
---+---+---
 X | O | 6
---+---+---
 X | 8 | O
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 6</summary><pre>
 O | X | 3
---+---+---
 4 | O | X
---+---+---
 X | 8 | O
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 8</summary><pre>
 O | X | 3
---+---+---
 4 | O | 6
---+---+---
 X | X | O
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 9</summary><pre>
 O | X | 3
---+---+---
 4 | O | 6
---+---+---
 X | O | X
</pre>
O responds at 8. Your move:
<details><summary>Play X at 3</summary><pre>
 O | X | X
---+---+---
 4 | O | O
---+---+---
 X | O | X
</pre>
O responds at 6. Your move:
<details><summary>Play X at 4</summary><pre>
 O | X | X
---+---+---
 X | O | O
---+---+---
 X | O | X
</pre><b>Draw. Best possible result against a perfect opponent.</b>
</details>
</details>
<details><summary>Play X at 4</summary><pre>
 O | X | O
---+---+---
 X | O | 6
---+---+---
 X | O | X
</pre>
O responds at 3. Your move:
<details><summary>Play X at 6</summary><pre>
 O | X | O
---+---+---
 X | O | X
---+---+---
 X | O | X
</pre><b>Draw. Best possible result against a perfect opponent.</b>
</details>
</details>
<details><summary>Play X at 6</summary><pre>
 O | X | O
---+---+---
 4 | O | X
---+---+---
 X | O | X
</pre>
O responds at 3. Your move:
<details><summary>Play X at 4</summary><pre>
 O | X | O
---+---+---
 X | O | X
---+---+---
 X | O | X
</pre><b>Draw. Best possible result against a perfect opponent.</b>
</details>
</details>
</details>
</details>
<details><summary>Play X at 8</summary><pre>
 O | X | 3
---+---+---
 4 | O | 6
---+---+---
 7 | X | 9
</pre>
O responds at 5. Your move:
<details><summary>Play X at 3</summary><pre>
 O | X | X
---+---+---
 O | O | 6
---+---+---
 7 | X | 9
</pre>
O responds at 4. Your move:
<details><summary>Play X at 6</summary><pre>
 O | X | X
---+---+---
 O | O | X
---+---+---
 O | X | 9
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 7</summary><pre>
 O | X | X
---+---+---
 O | O | O
---+---+---
 X | X | 9
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 9</summary><pre>
 O | X | X
---+---+---
 O | O | O
---+---+---
 7 | X | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
</details>
<details><summary>Play X at 4</summary><pre>
 O | X | O
---+---+---
 X | O | 6
---+---+---
 7 | X | 9
</pre>
O responds at 3. Your move:
<details><summary>Play X at 6</summary><pre>
 O | X | O
---+---+---
 X | O | X
---+---+---
 O | X | 9
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 7</summary><pre>
 O | X | O
---+---+---
 X | O | 6
---+---+---
 X | X | O
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 9</summary><pre>
 O | X | O
---+---+---
 X | O | 6
---+---+---
 O | X | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
</details>
<details><summary>Play X at 6</summary><pre>
 O | X | O
---+---+---
 4 | O | X
---+---+---
 7 | X | 9
</pre>
O responds at 3. Your move:
<details><summary>Play X at 4</summary><pre>
 O | X | O
---+---+---
 X | O | X
---+---+---
 O | X | 9
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 7</summary><pre>
 O | X | O
---+---+---
 4 | O | X
---+---+---
 X | X | O
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 9</summary><pre>
 O | X | O
---+---+---
 4 | O | X
---+---+---
 O | X | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
</details>
<details><summary>Play X at 7</summary><pre>
 O | X | 3
---+---+---
 4 | O | 6
---+---+---
 X | X | O
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 9</summary><pre>
 O | X | 3
---+---+---
 4 | O | 6
---+---+---
 O | X | X
</pre>
O responds at 7. Your move:
<details><summary>Play X at 3</summary><pre>
 O | X | X
---+---+---
 O | O | 6
---+---+---
 O | X | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 4</summary><pre>
 O | X | O
---+---+---
 X | O | 6
---+---+---
 O | X | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 6</summary><pre>
 O | X | O
---+---+---
 4 | O | X
---+---+---
 O | X | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
</details>
</details>
<details><summary>Play X at 9</summary><pre>
 O | X | 3
---+---+---
 4 | O | 6
---+---+---
 7 | 8 | X
</pre>
O responds at 5. Your move:
<details><summary>Play X at 3</summary><pre>
 O | X | X
---+---+---
 4 | O | O
---+---+---
 7 | 8 | X
</pre>
O responds at 6. Your move:
<details><summary>Play X at 4</summary><pre>
 O | X | X
---+---+---
 X | O | O
---+---+---
 O | 8 | X
</pre>
O responds at 7. Your move:
<details><summary>Play X at 8</summary><pre>
 O | X | X
---+---+---
 X | O | O
---+---+---
 O | X | X
</pre><b>Draw. Best possible result against a perfect opponent.</b>
</details>
</details>
<details><summary>Play X at 7</summary><pre>
 O | X | X
---+---+---
 O | O | O
---+---+---
 X | 8 | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 8</summary><pre>
 O | X | X
---+---+---
 O | O | O
---+---+---
 7 | X | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
</details>
<details><summary>Play X at 4</summary><pre>
 O | X | O
---+---+---
 X | O | 6
---+---+---
 7 | 8 | X
</pre>
O responds at 3. Your move:
<details><summary>Play X at 6</summary><pre>
 O | X | O
---+---+---
 X | O | X
---+---+---
 O | 8 | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 7</summary><pre>
 O | X | O
---+---+---
 X | O | 6
---+---+---
 X | O | X
</pre>
O responds at 8. Your move:
<details><summary>Play X at 6</summary><pre>
 O | X | O
---+---+---
 X | O | X
---+---+---
 X | O | X
</pre><b>Draw. Best possible result against a perfect opponent.</b>
</details>
</details>
<details><summary>Play X at 8</summary><pre>
 O | X | O
---+---+---
 X | O | 6
---+---+---
 O | X | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
</details>
<details><summary>Play X at 6</summary><pre>
 O | X | O
---+---+---
 4 | O | X
---+---+---
 7 | 8 | X
</pre>
O responds at 3. Your move:
<details><summary>Play X at 4</summary><pre>
 O | X | O
---+---+---
 X | O | X
---+---+---
 O | 8 | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 7</summary><pre>
 O | X | O
---+---+---
 4 | O | X
---+---+---
 X | O | X
</pre>
O responds at 8. Your move:
<details><summary>Play X at 4</summary><pre>
 O | X | O
---+---+---
 X | O | X
---+---+---
 X | O | X
</pre><b>Draw. Best possible result against a perfect opponent.</b>
</details>
</details>
<details><summary>Play X at 8</summary><pre>
 O | X | O
---+---+---
 4 | O | X
---+---+---
 O | X | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
</details>
<details><summary>Play X at 7</summary><pre>
 O | X | 3
---+---+---
 4 | O | 6
---+---+---
 X | O | X
</pre>
O responds at 8. Your move:
<details><summary>Play X at 3</summary><pre>
 O | X | X
---+---+---
 4 | O | O
---+---+---
 X | O | X
</pre>
O responds at 6. Your move:
<details><summary>Play X at 4</summary><pre>
 O | X | X
---+---+---
 X | O | O
---+---+---
 X | O | X
</pre><b>Draw. Best possible result against a perfect opponent.</b>
</details>
</details>
<details><summary>Play X at 4</summary><pre>
 O | X | O
---+---+---
 X | O | 6
---+---+---
 X | O | X
</pre>
O responds at 3. Your move:
<details><summary>Play X at 6</summary><pre>
 O | X | O
---+---+---
 X | O | X
---+---+---
 X | O | X
</pre><b>Draw. Best possible result against a perfect opponent.</b>
</details>
</details>
<details><summary>Play X at 6</summary><pre>
 O | X | O
---+---+---
 4 | O | X
---+---+---
 X | O | X
</pre>
O responds at 3. Your move:
<details><summary>Play X at 4</summary><pre>
 O | X | O
---+---+---
 X | O | X
---+---+---
 X | O | X
</pre><b>Draw. Best possible result against a perfect opponent.</b>
</details>
</details>
</details>
<details><summary>Play X at 8</summary><pre>
 O | X | 3
---+---+---
 4 | O | 6
---+---+---
 O | X | X
</pre>
O responds at 7. Your move:
<details><summary>Play X at 3</summary><pre>
 O | X | X
---+---+---
 O | O | 6
---+---+---
 O | X | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 4</summary><pre>
 O | X | O
---+---+---
 X | O | 6
---+---+---
 O | X | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 6</summary><pre>
 O | X | O
---+---+---
 4 | O | X
---+---+---
 O | X | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
</details>
</details>
</details>
<details><summary>Play X at 3</summary><pre>
 1 | 2 | X
---+---+---
 4 | O | 6
---+---+---
 7 | 8 | 9
</pre>
O responds at 5. Your move:
<details><summary>Play X at 1</summary><pre>
 X | O | X
---+---+---
 4 | O | 6
---+---+---
 7 | 8 | 9
</pre>
O responds at 2. Your move:
<details><summary>Play X at 4</summary><pre>
 X | O | X
---+---+---
 X | O | 6
---+---+---
 7 | O | 9
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 6</summary><pre>
 X | O | X
---+---+---
 4 | O | X
---+---+---
 7 | O | 9
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 7</summary><pre>
 X | O | X
---+---+---
 O | O | 6
---+---+---
 X | 8 | 9
</pre>
O responds at 4. Your move:
<details><summary>Play X at 6</summary><pre>
 X | O | X
---+---+---
 O | O | X
---+---+---
 X | O | 9
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 8</summary><pre>
 X | O | X
---+---+---
 O | O | O
---+---+---
 X | X | 9
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 9</summary><pre>
 X | O | X
---+---+---
 O | O | O
---+---+---
 X | 8 | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
</details>
<details><summary>Play X at 8</summary><pre>
 X | O | X
---+---+---
 O | O | 6
---+---+---
 7 | X | 9
</pre>
O responds at 4. Your move:
<details><summary>Play X at 6</summary><pre>
 X | O | X
---+---+---
 O | O | X
---+---+---
 7 | X | O
</pre>
O responds at 9. Your move:
<details><summary>Play X at 7</summary><pre>
 X | O | X
---+---+---
 O | O | X
---+---+---
 X | X | O
</pre><b>Draw. Best possible result against a perfect opponent.</b>
</details>
</details>
<details><summary>Play X at 7</summary><pre>
 X | O | X
---+---+---
 O | O | O
---+---+---
 X | X | 9
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 9</summary><pre>
 X | O | X
---+---+---
 O | O | O
---+---+---
 7 | X | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
</details>
<details><summary>Play X at 9</summary><pre>
 X | O | X
---+---+---
 4 | O | O
---+---+---
 7 | 8 | X
</pre>
O responds at 6. Your move:
<details><summary>Play X at 4</summary><pre>
 X | O | X
---+---+---
 X | O | O
---+---+---
 7 | O | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 7</summary><pre>
 X | O | X
---+---+---
 O | O | O
---+---+---
 X | 8 | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 8</summary><pre>
 X | O | X
---+---+---
 O | O | O
---+---+---
 7 | X | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
</details>
</details>
<details><summary>Play X at 2</summary><pre>
 O | X | X
---+---+---
 4 | O | 6
---+---+---
 7 | 8 | 9
</pre>
O responds at 1. Your move:
<details><summary>Play X at 4</summary><pre>
 O | X | X
---+---+---
 X | O | 6
---+---+---
 7 | 8 | O
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 6</summary><pre>
 O | X | X
---+---+---
 4 | O | X
---+---+---
 7 | 8 | O
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 7</summary><pre>
 O | X | X
---+---+---
 O | O | 6
---+---+---
 X | 8 | 9
</pre>
O responds at 4. Your move:
<details><summary>Play X at 6</summary><pre>
 O | X | X
---+---+---
 O | O | X
---+---+---
 X | 8 | O
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 8</summary><pre>
 O | X | X
---+---+---
 O | O | O
---+---+---
 X | X | 9
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 9</summary><pre>
 O | X | X
---+---+---
 O | O | O
---+---+---
 X | 8 | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
</details>
<details><summary>Play X at 8</summary><pre>
 O | X | X
---+---+---
 O | O | 6
---+---+---
 7 | X | 9
</pre>
O responds at 4. Your move:
<details><summary>Play X at 6</summary><pre>
 O | X | X
---+---+---
 O | O | X
---+---+---
 O | X | 9
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 7</summary><pre>
 O | X | X
---+---+---
 O | O | O
---+---+---
 X | X | 9
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 9</summary><pre>
 O | X | X
---+---+---
 O | O | O
---+---+---
 7 | X | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
</details>
<details><summary>Play X at 9</summary><pre>
 O | X | X
---+---+---
 4 | O | O
---+---+---
 7 | 8 | X
</pre>
O responds at 6. Your move:
<details><summary>Play X at 4</summary><pre>
 O | X | X
---+---+---
 X | O | O
---+---+---
 O | 8 | X
</pre>
O responds at 7. Your move:
<details><summary>Play X at 8</summary><pre>
 O | X | X
---+---+---
 X | O | O
---+---+---
 O | X | X
</pre><b>Draw. Best possible result against a perfect opponent.</b>
</details>
</details>
<details><summary>Play X at 7</summary><pre>
 O | X | X
---+---+---
 O | O | O
---+---+---
 X | 8 | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 8</summary><pre>
 O | X | X
---+---+---
 O | O | O
---+---+---
 7 | X | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
</details>
</details>
<details><summary>Play X at 4</summary><pre>
 O | 2 | X
---+---+---
 X | O | 6
---+---+---
 7 | 8 | 9
</pre>
O responds at 1. Your move:
<details><summary>Play X at 2</summary><pre>
 O | X | X
---+---+---
 X | O | 6
---+---+---
 7 | 8 | O
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 6</summary><pre>
 O | 2 | X
---+---+---
 X | O | X
---+---+---
 7 | 8 | O
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 7</summary><pre>
 O | O | X
---+---+---
 X | O | 6
---+---+---
 X | 8 | 9
</pre>
O responds at 2. Your move:
<details><summary>Play X at 6</summary><pre>
 O | O | X
---+---+---
 X | O | X
---+---+---
 X | O | 9
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 8</summary><pre>
 O | O | X
---+---+---
 X | O | 6
---+---+---
 X | X | O
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 9</summary><pre>
 O | O | X
---+---+---
 X | O | 6
---+---+---
 X | O | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
</details>
<details><summary>Play X at 8</summary><pre>
 O | 2 | X
---+---+---
 X | O | 6
---+---+---
 7 | X | O
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 9</summary><pre>
 O | 2 | X
---+---+---
 X | O | O
---+---+---
 7 | 8 | X
</pre>
O responds at 6. Your move:
<details><summary>Play X at 2</summary><pre>
 O | X | X
---+---+---
 X | O | O
---+---+---
 O | 8 | X
</pre>
O responds at 7. Your move:
<details><summary>Play X at 8</summary><pre>
 O | X | X
---+---+---
 X | O | O
---+---+---
 O | X | X
</pre><b>Draw. Best possible result against a perfect opponent.</b>
</details>
</details>
<details><summary>Play X at 7</summary><pre>
 O | 2 | X
---+---+---
 X | O | O
---+---+---
 X | O | X
</pre>
O responds at 8. Your move:
<details><summary>Play X at 2</summary><pre>
 O | X | X
---+---+---
 X | O | O
---+---+---
 X | O | X
</pre><b>Draw. Best possible result against a perfect opponent.</b>
</details>
</details>
<details><summary>Play X at 8</summary><pre>
 O | 2 | X
---+---+---
 X | O | O
---+---+---
 O | X | X
</pre>
O responds at 7. Your move:
<details><summary>Play X at 2</summary><pre>
 O | X | X
---+---+---
 X | O | O
---+---+---
 O | X | X
</pre><b>Draw. Best possible result against a perfect opponent.</b>
</details>
</details>
</details>
</details>
<details><summary>Play X at 6</summary><pre>
 1 | 2 | X
---+---+---
 4 | O | X
---+---+---
 7 | 8 | O
</pre>
O responds at 9. Your move:
<details><summary>Play X at 1</summary><pre>
 X | O | X
---+---+---
 4 | O | X
---+---+---
 7 | 8 | O
</pre>
O responds at 2. Your move:
<details><summary>Play X at 4</summary><pre>
 X | O | X
---+---+---
 X | O | X
---+---+---
 7 | O | O
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 7</summary><pre>
 X | O | X
---+---+---
 4 | O | X
---+---+---
 X | O | O
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 8</summary><pre>
 X | O | X
---+---+---
 O | O | X
---+---+---
 7 | X | O
</pre>
O responds at 4. Your move:
<details><summary>Play X at 7</summary><pre>
 X | O | X
---+---+---
 O | O | X
---+---+---
 X | X | O
</pre><b>Draw. Best possible result against a perfect opponent.</b>
</details>
</details>
</details>
<details><summary>Play X at 2</summary><pre>
 O | X | X
---+---+---
 4 | O | X
---+---+---
 7 | 8 | O
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 4</summary><pre>
 O | 2 | X
---+---+---
 X | O | X
---+---+---
 7 | 8 | O
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 7</summary><pre>
 O | 2 | X
---+---+---
 4 | O | X
---+---+---
 X | 8 | O
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 8</summary><pre>
 O | 2 | X
---+---+---
 4 | O | X
---+---+---
 7 | X | O
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
</details>
<details><summary>Play X at 7</summary><pre>
 1 | O | X
---+---+---
 4 | O | 6
---+---+---
 X | 8 | 9
</pre>
O responds at 2. Your move:
<details><summary>Play X at 1</summary><pre>
 X | O | X
---+---+---
 O | O | 6
---+---+---
 X | 8 | 9
</pre>
O responds at 4. Your move:
<details><summary>Play X at 6</summary><pre>
 X | O | X
---+---+---
 O | O | X
---+---+---
 X | O | 9
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 8</summary><pre>
 X | O | X
---+---+---
 O | O | O
---+---+---
 X | X | 9
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 9</summary><pre>
 X | O | X
---+---+---
 O | O | O
---+---+---
 X | 8 | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
</details>
<details><summary>Play X at 4</summary><pre>
 O | O | X
---+---+---
 X | O | 6
---+---+---
 X | 8 | 9
</pre>
O responds at 1. Your move:
<details><summary>Play X at 6</summary><pre>
 O | O | X
---+---+---
 X | O | X
---+---+---
 X | O | 9
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 8</summary><pre>
 O | O | X
---+---+---
 X | O | 6
---+---+---
 X | X | O
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 9</summary><pre>
 O | O | X
---+---+---
 X | O | 6
---+---+---
 X | O | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
</details>
<details><summary>Play X at 6</summary><pre>
 1 | O | X
---+---+---
 4 | O | X
---+---+---
 X | O | 9
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 8</summary><pre>
 1 | O | X
---+---+---
 4 | O | 6
---+---+---
 X | X | O
</pre>
O responds at 9. Your move:
<details><summary>Play X at 1</summary><pre>
 X | O | X
---+---+---
 O | O | 6
---+---+---
 X | X | O
</pre>
O responds at 4. Your move:
<details><summary>Play X at 6</summary><pre>
 X | O | X
---+---+---
 O | O | X
---+---+---
 X | X | O
</pre><b>Draw. Best possible result against a perfect opponent.</b>
</details>
</details>
<details><summary>Play X at 4</summary><pre>
 O | O | X
---+---+---
 X | O | 6
---+---+---
 X | X | O
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 6</summary><pre>
 O | O | X
---+---+---
 4 | O | X
---+---+---
 X | X | O
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
</details>
<details><summary>Play X at 9</summary><pre>
 1 | O | X
---+---+---
 4 | O | 6
---+---+---
 X | O | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
</details>
<details><summary>Play X at 8</summary><pre>
 1 | 2 | X
---+---+---
 O | O | 6
---+---+---
 7 | X | 9
</pre>
O responds at 4. Your move:
<details><summary>Play X at 1</summary><pre>
 X | 2 | X
---+---+---
 O | O | O
---+---+---
 7 | X | 9
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 2</summary><pre>
 O | X | X
---+---+---
 O | O | 6
---+---+---
 7 | X | 9
</pre>
O responds at 1. Your move:
<details><summary>Play X at 6</summary><pre>
 O | X | X
---+---+---
 O | O | X
---+---+---
 O | X | 9
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 7</summary><pre>
 O | X | X
---+---+---
 O | O | O
---+---+---
 X | X | 9
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 9</summary><pre>
 O | X | X
---+---+---
 O | O | O
---+---+---
 7 | X | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
</details>
<details><summary>Play X at 6</summary><pre>
 1 | 2 | X
---+---+---
 O | O | X
---+---+---
 7 | X | O
</pre>
O responds at 9. Your move:
<details><summary>Play X at 1</summary><pre>
 X | O | X
---+---+---
 O | O | X
---+---+---
 7 | X | O
</pre>
O responds at 2. Your move:
<details><summary>Play X at 7</summary><pre>
 X | O | X
---+---+---
 O | O | X
---+---+---
 X | X | O
</pre><b>Draw. Best possible result against a perfect opponent.</b>
</details>
</details>
<details><summary>Play X at 2</summary><pre>
 O | X | X
---+---+---
 O | O | X
---+---+---
 7 | X | O
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 7</summary><pre>
 O | 2 | X
---+---+---
 O | O | X
---+---+---
 X | X | O
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
</details>
<details><summary>Play X at 7</summary><pre>
 1 | 2 | X
---+---+---
 O | O | O
---+---+---
 X | X | 9
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 9</summary><pre>
 1 | 2 | X
---+---+---
 O | O | O
---+---+---
 7 | X | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
</details>
<details><summary>Play X at 9</summary><pre>
 1 | 2 | X
---+---+---
 4 | O | O
---+---+---
 7 | 8 | X
</pre>
O responds at 6. Your move:
<details><summary>Play X at 1</summary><pre>
 X | O | X
---+---+---
 4 | O | O
---+---+---
 7 | 8 | X
</pre>
O responds at 2. Your move:
<details><summary>Play X at 4</summary><pre>
 X | O | X
---+---+---
 X | O | O
---+---+---
 7 | O | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 7</summary><pre>
 X | O | X
---+---+---
 O | O | O
---+---+---
 X | 8 | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 8</summary><pre>
 X | O | X
---+---+---
 O | O | O
---+---+---
 7 | X | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
</details>
<details><summary>Play X at 2</summary><pre>
 1 | X | X
---+---+---
 O | O | O
---+---+---
 7 | 8 | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 4</summary><pre>
 O | 2 | X
---+---+---
 X | O | O
---+---+---
 7 | 8 | X
</pre>
O responds at 1. Your move:
<details><summary>Play X at 2</summary><pre>
 O | X | X
---+---+---
 X | O | O
---+---+---
 O | 8 | X
</pre>
O responds at 7. Your move:
<details><summary>Play X at 8</summary><pre>
 O | X | X
---+---+---
 X | O | O
---+---+---
 O | X | X
</pre><b>Draw. Best possible result against a perfect opponent.</b>
</details>
</details>
<details><summary>Play X at 7</summary><pre>
 O | 2 | X
---+---+---
 X | O | O
---+---+---
 X | O | X
</pre>
O responds at 8. Your move:
<details><summary>Play X at 2</summary><pre>
 O | X | X
---+---+---
 X | O | O
---+---+---
 X | O | X
</pre><b>Draw. Best possible result against a perfect opponent.</b>
</details>
</details>
<details><summary>Play X at 8</summary><pre>
 O | 2 | X
---+---+---
 X | O | O
---+---+---
 O | X | X
</pre>
O responds at 7. Your move:
<details><summary>Play X at 2</summary><pre>
 O | X | X
---+---+---
 X | O | O
---+---+---
 O | X | X
</pre><b>Draw. Best possible result against a perfect opponent.</b>
</details>
</details>
</details>
<details><summary>Play X at 7</summary><pre>
 1 | 2 | X
---+---+---
 O | O | O
---+---+---
 X | 8 | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 8</summary><pre>
 1 | 2 | X
---+---+---
 O | O | O
---+---+---
 7 | X | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
</details>
</details>
<details><summary>Play X at 4</summary><pre>
 O | 2 | 3
---+---+---
 X | 5 | 6
---+---+---
 7 | 8 | 9
</pre>
O responds at 1. Your move:
<details><summary>Play X at 2</summary><pre>
 O | X | 3
---+---+---
 X | O | 6
---+---+---
 7 | 8 | 9
</pre>
O responds at 5. Your move:
<details><summary>Play X at 3</summary><pre>
 O | X | X
---+---+---
 X | O | 6
---+---+---
 7 | 8 | O
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 6</summary><pre>
 O | X | O
---+---+---
 X | O | X
---+---+---
 7 | 8 | 9
</pre>
O responds at 3. Your move:
<details><summary>Play X at 7</summary><pre>
 O | X | O
---+---+---
 X | O | X
---+---+---
 X | 8 | O
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 8</summary><pre>
 O | X | O
---+---+---
 X | O | X
---+---+---
 O | X | 9
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 9</summary><pre>
 O | X | O
---+---+---
 X | O | X
---+---+---
 O | 8 | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
</details>
<details><summary>Play X at 7</summary><pre>
 O | X | 3
---+---+---
 X | O | 6
---+---+---
 X | 8 | O
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 8</summary><pre>
 O | X | O
---+---+---
 X | O | 6
---+---+---
 7 | X | 9
</pre>
O responds at 3. Your move:
<details><summary>Play X at 6</summary><pre>
 O | X | O
---+---+---
 X | O | X
---+---+---
 O | X | 9
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 7</summary><pre>
 O | X | O
---+---+---
 X | O | 6
---+---+---
 X | X | O
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 9</summary><pre>
 O | X | O
---+---+---
 X | O | 6
---+---+---
 O | X | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
</details>
<details><summary>Play X at 9</summary><pre>
 O | X | O
---+---+---
 X | O | 6
---+---+---
 7 | 8 | X
</pre>
O responds at 3. Your move:
<details><summary>Play X at 6</summary><pre>
 O | X | O
---+---+---
 X | O | X
---+---+---
 O | 8 | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 7</summary><pre>
 O | X | O
---+---+---
 X | O | 6
---+---+---
 X | O | X
</pre>
O responds at 8. Your move:
<details><summary>Play X at 6</summary><pre>
 O | X | O
---+---+---
 X | O | X
---+---+---
 X | O | X
</pre><b>Draw. Best possible result against a perfect opponent.</b>
</details>
</details>
<details><summary>Play X at 8</summary><pre>
 O | X | O
---+---+---
 X | O | 6
---+---+---
 O | X | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
</details>
</details>
<details><summary>Play X at 3</summary><pre>
 O | 2 | X
---+---+---
 X | O | 6
---+---+---
 7 | 8 | 9
</pre>
O responds at 5. Your move:
<details><summary>Play X at 2</summary><pre>
 O | X | X
---+---+---
 X | O | 6
---+---+---
 7 | 8 | O
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 6</summary><pre>
 O | 2 | X
---+---+---
 X | O | X
---+---+---
 7 | 8 | O
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 7</summary><pre>
 O | O | X
---+---+---
 X | O | 6
---+---+---
 X | 8 | 9
</pre>
O responds at 2. Your move:
<details><summary>Play X at 6</summary><pre>
 O | O | X
---+---+---
 X | O | X
---+---+---
 X | O | 9
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 8</summary><pre>
 O | O | X
---+---+---
 X | O | 6
---+---+---
 X | X | O
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 9</summary><pre>
 O | O | X
---+---+---
 X | O | 6
---+---+---
 X | O | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
</details>
<details><summary>Play X at 8</summary><pre>
 O | 2 | X
---+---+---
 X | O | 6
---+---+---
 7 | X | O
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 9</summary><pre>
 O | 2 | X
---+---+---
 X | O | O
---+---+---
 7 | 8 | X
</pre>
O responds at 6. Your move:
<details><summary>Play X at 2</summary><pre>
 O | X | X
---+---+---
 X | O | O
---+---+---
 O | 8 | X
</pre>
O responds at 7. Your move:
<details><summary>Play X at 8</summary><pre>
 O | X | X
---+---+---
 X | O | O
---+---+---
 O | X | X
</pre><b>Draw. Best possible result against a perfect opponent.</b>
</details>
</details>
<details><summary>Play X at 7</summary><pre>
 O | 2 | X
---+---+---
 X | O | O
---+---+---
 X | O | X
</pre>
O responds at 8. Your move:
<details><summary>Play X at 2</summary><pre>
 O | X | X
---+---+---
 X | O | O
---+---+---
 X | O | X
</pre><b>Draw. Best possible result against a perfect opponent.</b>
</details>
</details>
<details><summary>Play X at 8</summary><pre>
 O | 2 | X
---+---+---
 X | O | O
---+---+---
 O | X | X
</pre>
O responds at 7. Your move:
<details><summary>Play X at 2</summary><pre>
 O | X | X
---+---+---
 X | O | O
---+---+---
 O | X | X
</pre><b>Draw. Best possible result against a perfect opponent.</b>
</details>
</details>
</details>
</details>
<details><summary>Play X at 5</summary><pre>
 O | 2 | 3
---+---+---
 X | X | O
---+---+---
 7 | 8 | 9
</pre>
O responds at 6. Your move:
<details><summary>Play X at 2</summary><pre>
 O | X | 3
---+---+---
 X | X | O
---+---+---
 7 | O | 9
</pre>
O responds at 8. Your move:
<details><summary>Play X at 3</summary><pre>
 O | X | X
---+---+---
 X | X | O
---+---+---
 O | O | 9
</pre>
O responds at 7. Your move:
<details><summary>Play X at 9</summary><pre>
 O | X | X
---+---+---
 X | X | O
---+---+---
 O | O | X
</pre><b>Draw. Best possible result against a perfect opponent.</b>
</details>
</details>
<details><summary>Play X at 7</summary><pre>
 O | X | O
---+---+---
 X | X | O
---+---+---
 X | O | 9
</pre>
O responds at 3. Your move:
<details><summary>Play X at 9</summary><pre>
 O | X | O
---+---+---
 X | X | O
---+---+---
 X | O | X
</pre><b>Draw. Best possible result against a perfect opponent.</b>
</details>
</details>
<details><summary>Play X at 9</summary><pre>
 O | X | O
---+---+---
 X | X | O
---+---+---
 7 | O | X
</pre>
O responds at 3. Your move:
<details><summary>Play X at 7</summary><pre>
 O | X | O
---+---+---
 X | X | O
---+---+---
 X | O | X
</pre><b>Draw. Best possible result against a perfect opponent.</b>
</details>
</details>
</details>
<details><summary>Play X at 3</summary><pre>
 O | 2 | X
---+---+---
 X | X | O
---+---+---
 O | 8 | 9
</pre>
O responds at 7. Your move:
<details><summary>Play X at 2</summary><pre>
 O | X | X
---+---+---
 X | X | O
---+---+---
 O | O | 9
</pre>
O responds at 8. Your move:
<details><summary>Play X at 9</summary><pre>
 O | X | X
---+---+---
 X | X | O
---+---+---
 O | O | X
</pre><b>Draw. Best possible result against a perfect opponent.</b>
</details>
</details>
<details><summary>Play X at 8</summary><pre>
 O | O | X
---+---+---
 X | X | O
---+---+---
 O | X | 9
</pre>
O responds at 2. Your move:
<details><summary>Play X at 9</summary><pre>
 O | O | X
---+---+---
 X | X | O
---+---+---
 O | X | X
</pre><b>Draw. Best possible result against a perfect opponent.</b>
</details>
</details>
<details><summary>Play X at 9</summary><pre>
 O | O | X
---+---+---
 X | X | O
---+---+---
 O | 8 | X
</pre>
O responds at 2. Your move:
<details><summary>Play X at 8</summary><pre>
 O | O | X
---+---+---
 X | X | O
---+---+---
 O | X | X
</pre><b>Draw. Best possible result against a perfect opponent.</b>
</details>
</details>
</details>
<details><summary>Play X at 7</summary><pre>
 O | 2 | O
---+---+---
 X | X | O
---+---+---
 X | 8 | 9
</pre>
O responds at 3. Your move:
<details><summary>Play X at 2</summary><pre>
 O | X | O
---+---+---
 X | X | O
---+---+---
 X | 8 | O
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 8</summary><pre>
 O | O | O
---+---+---
 X | X | O
---+---+---
 X | X | 9
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 9</summary><pre>
 O | O | O
---+---+---
 X | X | O
---+---+---
 X | 8 | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
</details>
<details><summary>Play X at 8</summary><pre>
 O | O | 3
---+---+---
 X | X | O
---+---+---
 7 | X | 9
</pre>
O responds at 2. Your move:
<details><summary>Play X at 3</summary><pre>
 O | O | X
---+---+---
 X | X | O
---+---+---
 O | X | 9
</pre>
O responds at 7. Your move:
<details><summary>Play X at 9</summary><pre>
 O | O | X
---+---+---
 X | X | O
---+---+---
 O | X | X
</pre><b>Draw. Best possible result against a perfect opponent.</b>
</details>
</details>
<details><summary>Play X at 7</summary><pre>
 O | O | O
---+---+---
 X | X | O
---+---+---
 X | X | 9
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 9</summary><pre>
 O | O | O
---+---+---
 X | X | O
---+---+---
 7 | X | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
</details>
<details><summary>Play X at 9</summary><pre>
 O | O | 3
---+---+---
 X | X | O
---+---+---
 7 | 8 | X
</pre>
O responds at 2. Your move:
<details><summary>Play X at 3</summary><pre>
 O | O | X
---+---+---
 X | X | O
---+---+---
 O | 8 | X
</pre>
O responds at 7. Your move:
<details><summary>Play X at 8</summary><pre>
 O | O | X
---+---+---
 X | X | O
---+---+---
 O | X | X
</pre><b>Draw. Best possible result against a perfect opponent.</b>
</details>
</details>
<details><summary>Play X at 7</summary><pre>
 O | O | O
---+---+---
 X | X | O
---+---+---
 X | 8 | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 8</summary><pre>
 O | O | O
---+---+---
 X | X | O
---+---+---
 7 | X | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
</details>
</details>
<details><summary>Play X at 6</summary><pre>
 O | 2 | 3
---+---+---
 X | O | X
---+---+---
 7 | 8 | 9
</pre>
O responds at 5. Your move:
<details><summary>Play X at 2</summary><pre>
 O | X | O
---+---+---
 X | O | X
---+---+---
 7 | 8 | 9
</pre>
O responds at 3. Your move:
<details><summary>Play X at 7</summary><pre>
 O | X | O
---+---+---
 X | O | X
---+---+---
 X | 8 | O
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 8</summary><pre>
 O | X | O
---+---+---
 X | O | X
---+---+---
 O | X | 9
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 9</summary><pre>
 O | X | O
---+---+---
 X | O | X
---+---+---
 O | 8 | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
</details>
<details><summary>Play X at 3</summary><pre>
 O | 2 | X
---+---+---
 X | O | X
---+---+---
 7 | 8 | O
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 7</summary><pre>
 O | O | 3
---+---+---
 X | O | X
---+---+---
 X | 8 | 9
</pre>
O responds at 2. Your move:
<details><summary>Play X at 3</summary><pre>
 O | O | X
---+---+---
 X | O | X
---+---+---
 X | O | 9
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 8</summary><pre>
 O | O | O
---+---+---
 X | O | X
---+---+---
 X | X | 9
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 9</summary><pre>
 O | O | O
---+---+---
 X | O | X
---+---+---
 X | 8 | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
</details>
<details><summary>Play X at 8</summary><pre>
 O | O | 3
---+---+---
 X | O | X
---+---+---
 7 | X | 9
</pre>
O responds at 2. Your move:
<details><summary>Play X at 3</summary><pre>
 O | O | X
---+---+---
 X | O | X
---+---+---
 7 | X | O
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 7</summary><pre>
 O | O | O
---+---+---
 X | O | X
---+---+---
 X | X | 9
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 9</summary><pre>
 O | O | O
---+---+---
 X | O | X
---+---+---
 7 | X | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
</details>
<details><summary>Play X at 9</summary><pre>
 O | 2 | O
---+---+---
 X | O | X
---+---+---
 7 | 8 | X
</pre>
O responds at 3. Your move:
<details><summary>Play X at 2</summary><pre>
 O | X | O
---+---+---
 X | O | X
---+---+---
 O | 8 | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 7</summary><pre>
 O | O | O
---+---+---
 X | O | X
---+---+---
 X | 8 | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 8</summary><pre>
 O | O | O
---+---+---
 X | O | X
---+---+---
 7 | X | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
</details>
</details>
<details><summary>Play X at 7</summary><pre>
 O | O | 3
---+---+---
 X | 5 | 6
---+---+---
 X | 8 | 9
</pre>
O responds at 2. Your move:
<details><summary>Play X at 3</summary><pre>
 O | O | X
---+---+---
 X | O | 6
---+---+---
 X | 8 | 9
</pre>
O responds at 5. Your move:
<details><summary>Play X at 6</summary><pre>
 O | O | X
---+---+---
 X | O | X
---+---+---
 X | O | 9
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 8</summary><pre>
 O | O | X
---+---+---
 X | O | 6
---+---+---
 X | X | O
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 9</summary><pre>
 O | O | X
---+---+---
 X | O | 6
---+---+---
 X | O | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
</details>
<details><summary>Play X at 5</summary><pre>
 O | O | O
---+---+---
 X | X | 6
---+---+---
 X | 8 | 9
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 6</summary><pre>
 O | O | O
---+---+---
 X | 5 | X
---+---+---
 X | 8 | 9
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 8</summary><pre>
 O | O | O
---+---+---
 X | 5 | 6
---+---+---
 X | X | 9
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 9</summary><pre>
 O | O | O
---+---+---
 X | 5 | 6
---+---+---
 X | 8 | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
</details>
<details><summary>Play X at 8</summary><pre>
 O | 2 | O
---+---+---
 X | 5 | 6
---+---+---
 7 | X | 9
</pre>
O responds at 3. Your move:
<details><summary>Play X at 2</summary><pre>
 O | X | O
---+---+---
 X | O | 6
---+---+---
 7 | X | 9
</pre>
O responds at 5. Your move:
<details><summary>Play X at 6</summary><pre>
 O | X | O
---+---+---
 X | O | X
---+---+---
 O | X | 9
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 7</summary><pre>
 O | X | O
---+---+---
 X | O | 6
---+---+---
 X | X | O
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 9</summary><pre>
 O | X | O
---+---+---
 X | O | 6
---+---+---
 O | X | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
</details>
<details><summary>Play X at 5</summary><pre>
 O | O | O
---+---+---
 X | X | 6
---+---+---
 7 | X | 9
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 6</summary><pre>
 O | O | O
---+---+---
 X | 5 | X
---+---+---
 7 | X | 9
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 7</summary><pre>
 O | O | O
---+---+---
 X | 5 | 6
---+---+---
 X | X | 9
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 9</summary><pre>
 O | O | O
---+---+---
 X | 5 | 6
---+---+---
 7 | X | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
</details>
<details><summary>Play X at 9</summary><pre>
 O | 2 | O
---+---+---
 X | 5 | 6
---+---+---
 7 | 8 | X
</pre>
O responds at 3. Your move:
<details><summary>Play X at 2</summary><pre>
 O | X | O
---+---+---
 X | O | 6
---+---+---
 7 | 8 | X
</pre>
O responds at 5. Your move:
<details><summary>Play X at 6</summary><pre>
 O | X | O
---+---+---
 X | O | X
---+---+---
 O | 8 | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 7</summary><pre>
 O | X | O
---+---+---
 X | O | 6
---+---+---
 X | O | X
</pre>
O responds at 8. Your move:
<details><summary>Play X at 6</summary><pre>
 O | X | O
---+---+---
 X | O | X
---+---+---
 X | O | X
</pre><b>Draw. Best possible result against a perfect opponent.</b>
</details>
</details>
<details><summary>Play X at 8</summary><pre>
 O | X | O
---+---+---
 X | O | 6
---+---+---
 O | X | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
</details>
<details><summary>Play X at 5</summary><pre>
 O | O | O
---+---+---
 X | X | 6
---+---+---
 7 | 8 | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 6</summary><pre>
 O | O | O
---+---+---
 X | 5 | X
---+---+---
 7 | 8 | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 7</summary><pre>
 O | O | O
---+---+---
 X | 5 | 6
---+---+---
 X | 8 | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 8</summary><pre>
 O | O | O
---+---+---
 X | 5 | 6
---+---+---
 7 | X | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
</details>
</details>
<details><summary>Play X at 5</summary><pre>
 O | 2 | 3
---+---+---
 4 | X | 6
---+---+---
 7 | 8 | 9
</pre>
O responds at 1. Your move:
<details><summary>Play X at 2</summary><pre>
 O | X | 3
---+---+---
 4 | X | 6
---+---+---
 7 | O | 9
</pre>
O responds at 8. Your move:
<details><summary>Play X at 3</summary><pre>
 O | X | X
---+---+---
 4 | X | 6
---+---+---
 O | O | 9
</pre>
O responds at 7. Your move:
<details><summary>Play X at 4</summary><pre>
 O | X | X
---+---+---
 X | X | 6
---+---+---
 O | O | O
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 6</summary><pre>
 O | X | X
---+---+---
 O | X | X
---+---+---
 O | O | 9
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 9</summary><pre>
 O | X | X
---+---+---
 O | X | 6
---+---+---
 O | O | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
</details>
<details><summary>Play X at 4</summary><pre>
 O | X | 3
---+---+---
 X | X | O
---+---+---
 7 | O | 9
</pre>
O responds at 6. Your move:
<details><summary>Play X at 3</summary><pre>
 O | X | X
---+---+---
 X | X | O
---+---+---
 O | O | 9
</pre>
O responds at 7. Your move:
<details><summary>Play X at 9</summary><pre>
 O | X | X
---+---+---
 X | X | O
---+---+---
 O | O | X
</pre><b>Draw. Best possible result against a perfect opponent.</b>
</details>
</details>
<details><summary>Play X at 7</summary><pre>
 O | X | O
---+---+---
 X | X | O
---+---+---
 X | O | 9
</pre>
O responds at 3. Your move:
<details><summary>Play X at 9</summary><pre>
 O | X | O
---+---+---
 X | X | O
---+---+---
 X | O | X
</pre><b>Draw. Best possible result against a perfect opponent.</b>
</details>
</details>
<details><summary>Play X at 9</summary><pre>
 O | X | O
---+---+---
 X | X | O
---+---+---
 7 | O | X
</pre>
O responds at 3. Your move:
<details><summary>Play X at 7</summary><pre>
 O | X | O
---+---+---
 X | X | O
---+---+---
 X | O | X
</pre><b>Draw. Best possible result against a perfect opponent.</b>
</details>
</details>
</details>
<details><summary>Play X at 6</summary><pre>
 O | X | 3
---+---+---
 O | X | X
---+---+---
 7 | O | 9
</pre>
O responds at 4. Your move:
<details><summary>Play X at 3</summary><pre>
 O | X | X
---+---+---
 O | X | X
---+---+---
 O | O | 9
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 7</summary><pre>
 O | X | O
---+---+---
 O | X | X
---+---+---
 X | O | 9
</pre>
O responds at 3. Your move:
<details><summary>Play X at 9</summary><pre>
 O | X | O
---+---+---
 O | X | X
---+---+---
 X | O | X
</pre><b>Draw. Best possible result against a perfect opponent.</b>
</details>
</details>
<details><summary>Play X at 9</summary><pre>
 O | X | 3
---+---+---
 O | X | X
---+---+---
 O | O | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
</details>
<details><summary>Play X at 7</summary><pre>
 O | X | O
---+---+---
 4 | X | 6
---+---+---
 X | O | 9
</pre>
O responds at 3. Your move:
<details><summary>Play X at 4</summary><pre>
 O | X | O
---+---+---
 X | X | O
---+---+---
 X | O | 9
</pre>
O responds at 6. Your move:
<details><summary>Play X at 9</summary><pre>
 O | X | O
---+---+---
 X | X | O
---+---+---
 X | O | X
</pre><b>Draw. Best possible result against a perfect opponent.</b>
</details>
</details>
<details><summary>Play X at 6</summary><pre>
 O | X | O
---+---+---
 O | X | X
---+---+---
 X | O | 9
</pre>
O responds at 4. Your move:
<details><summary>Play X at 9</summary><pre>
 O | X | O
---+---+---
 O | X | X
---+---+---
 X | O | X
</pre><b>Draw. Best possible result against a perfect opponent.</b>
</details>
</details>
<details><summary>Play X at 9</summary><pre>
 O | X | O
---+---+---
 O | X | 6
---+---+---
 X | O | X
</pre>
O responds at 4. Your move:
<details><summary>Play X at 6</summary><pre>
 O | X | O
---+---+---
 O | X | X
---+---+---
 X | O | X
</pre><b>Draw. Best possible result against a perfect opponent.</b>
</details>
</details>
</details>
<details><summary>Play X at 9</summary><pre>
 O | X | O
---+---+---
 4 | X | 6
---+---+---
 7 | O | X
</pre>
O responds at 3. Your move:
<details><summary>Play X at 4</summary><pre>
 O | X | O
---+---+---
 X | X | O
---+---+---
 7 | O | X
</pre>
O responds at 6. Your move:
<details><summary>Play X at 7</summary><pre>
 O | X | O
---+---+---
 X | X | O
---+---+---
 X | O | X
</pre><b>Draw. Best possible result against a perfect opponent.</b>
</details>
</details>
<details><summary>Play X at 6</summary><pre>
 O | X | O
---+---+---
 O | X | X
---+---+---
 7 | O | X
</pre>
O responds at 4. Your move:
<details><summary>Play X at 7</summary><pre>
 O | X | O
---+---+---
 O | X | X
---+---+---
 X | O | X
</pre><b>Draw. Best possible result against a perfect opponent.</b>
</details>
</details>
<details><summary>Play X at 7</summary><pre>
 O | X | O
---+---+---
 O | X | 6
---+---+---
 X | O | X
</pre>
O responds at 4. Your move:
<details><summary>Play X at 6</summary><pre>
 O | X | O
---+---+---
 O | X | X
---+---+---
 X | O | X
</pre><b>Draw. Best possible result against a perfect opponent.</b>
</details>
</details>
</details>
</details>
<details><summary>Play X at 3</summary><pre>
 O | 2 | X
---+---+---
 4 | X | 6
---+---+---
 O | 8 | 9
</pre>
O responds at 7. Your move:
<details><summary>Play X at 2</summary><pre>
 O | X | X
---+---+---
 O | X | 6
---+---+---
 O | 8 | 9
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 4</summary><pre>
 O | 2 | X
---+---+---
 X | X | O
---+---+---
 O | 8 | 9
</pre>
O responds at 6. Your move:
<details><summary>Play X at 2</summary><pre>
 O | X | X
---+---+---
 X | X | O
---+---+---
 O | O | 9
</pre>
O responds at 8. Your move:
<details><summary>Play X at 9</summary><pre>
 O | X | X
---+---+---
 X | X | O
---+---+---
 O | O | X
</pre><b>Draw. Best possible result against a perfect opponent.</b>
</details>
</details>
<details><summary>Play X at 8</summary><pre>
 O | O | X
---+---+---
 X | X | O
---+---+---
 O | X | 9
</pre>
O responds at 2. Your move:
<details><summary>Play X at 9</summary><pre>
 O | O | X
---+---+---
 X | X | O
---+---+---
 O | X | X
</pre><b>Draw. Best possible result against a perfect opponent.</b>
</details>
</details>
<details><summary>Play X at 9</summary><pre>
 O | O | X
---+---+---
 X | X | O
---+---+---
 O | 8 | X
</pre>
O responds at 2. Your move:
<details><summary>Play X at 8</summary><pre>
 O | O | X
---+---+---
 X | X | O
---+---+---
 O | X | X
</pre><b>Draw. Best possible result against a perfect opponent.</b>
</details>
</details>
</details>
<details><summary>Play X at 6</summary><pre>
 O | 2 | X
---+---+---
 O | X | X
---+---+---
 O | 8 | 9
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 8</summary><pre>
 O | 2 | X
---+---+---
 O | X | 6
---+---+---
 O | X | 9
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 9</summary><pre>
 O | 2 | X
---+---+---
 O | X | 6
---+---+---
 O | 8 | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
</details>
<details><summary>Play X at 4</summary><pre>
 O | 2 | 3
---+---+---
 X | X | O
---+---+---
 7 | 8 | 9
</pre>
O responds at 6. Your move:
<details><summary>Play X at 2</summary><pre>
 O | X | 3
---+---+---
 X | X | O
---+---+---
 7 | O | 9
</pre>
O responds at 8. Your move:
<details><summary>Play X at 3</summary><pre>
 O | X | X
---+---+---
 X | X | O
---+---+---
 O | O | 9
</pre>
O responds at 7. Your move:
<details><summary>Play X at 9</summary><pre>
 O | X | X
---+---+---
 X | X | O
---+---+---
 O | O | X
</pre><b>Draw. Best possible result against a perfect opponent.</b>
</details>
</details>
<details><summary>Play X at 7</summary><pre>
 O | X | O
---+---+---
 X | X | O
---+---+---
 X | O | 9
</pre>
O responds at 3. Your move:
<details><summary>Play X at 9</summary><pre>
 O | X | O
---+---+---
 X | X | O
---+---+---
 X | O | X
</pre><b>Draw. Best possible result against a perfect opponent.</b>
</details>
</details>
<details><summary>Play X at 9</summary><pre>
 O | X | O
---+---+---
 X | X | O
---+---+---
 7 | O | X
</pre>
O responds at 3. Your move:
<details><summary>Play X at 7</summary><pre>
 O | X | O
---+---+---
 X | X | O
---+---+---
 X | O | X
</pre><b>Draw. Best possible result against a perfect opponent.</b>
</details>
</details>
</details>
<details><summary>Play X at 3</summary><pre>
 O | 2 | X
---+---+---
 X | X | O
---+---+---
 O | 8 | 9
</pre>
O responds at 7. Your move:
<details><summary>Play X at 2</summary><pre>
 O | X | X
---+---+---
 X | X | O
---+---+---
 O | O | 9
</pre>
O responds at 8. Your move:
<details><summary>Play X at 9</summary><pre>
 O | X | X
---+---+---
 X | X | O
---+---+---
 O | O | X
</pre><b>Draw. Best possible result against a perfect opponent.</b>
</details>
</details>
<details><summary>Play X at 8</summary><pre>
 O | O | X
---+---+---
 X | X | O
---+---+---
 O | X | 9
</pre>
O responds at 2. Your move:
<details><summary>Play X at 9</summary><pre>
 O | O | X
---+---+---
 X | X | O
---+---+---
 O | X | X
</pre><b>Draw. Best possible result against a perfect opponent.</b>
</details>
</details>
<details><summary>Play X at 9</summary><pre>
 O | O | X
---+---+---
 X | X | O
---+---+---
 O | 8 | X
</pre>
O responds at 2. Your move:
<details><summary>Play X at 8</summary><pre>
 O | O | X
---+---+---
 X | X | O
---+---+---
 O | X | X
</pre><b>Draw. Best possible result against a perfect opponent.</b>
</details>
</details>
</details>
<details><summary>Play X at 7</summary><pre>
 O | 2 | O
---+---+---
 X | X | O
---+---+---
 X | 8 | 9
</pre>
O responds at 3. Your move:
<details><summary>Play X at 2</summary><pre>
 O | X | O
---+---+---
 X | X | O
---+---+---
 X | 8 | O
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 8</summary><pre>
 O | O | O
---+---+---
 X | X | O
---+---+---
 X | X | 9
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 9</summary><pre>
 O | O | O
---+---+---
 X | X | O
---+---+---
 X | 8 | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
</details>
<details><summary>Play X at 8</summary><pre>
 O | O | 3
---+---+---
 X | X | O
---+---+---
 7 | X | 9
</pre>
O responds at 2. Your move:
<details><summary>Play X at 3</summary><pre>
 O | O | X
---+---+---
 X | X | O
---+---+---
 O | X | 9
</pre>
O responds at 7. Your move:
<details><summary>Play X at 9</summary><pre>
 O | O | X
---+---+---
 X | X | O
---+---+---
 O | X | X
</pre><b>Draw. Best possible result against a perfect opponent.</b>
</details>
</details>
<details><summary>Play X at 7</summary><pre>
 O | O | O
---+---+---
 X | X | O
---+---+---
 X | X | 9
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 9</summary><pre>
 O | O | O
---+---+---
 X | X | O
---+---+---
 7 | X | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
</details>
<details><summary>Play X at 9</summary><pre>
 O | O | 3
---+---+---
 X | X | O
---+---+---
 7 | 8 | X
</pre>
O responds at 2. Your move:
<details><summary>Play X at 3</summary><pre>
 O | O | X
---+---+---
 X | X | O
---+---+---
 O | 8 | X
</pre>
O responds at 7. Your move:
<details><summary>Play X at 8</summary><pre>
 O | O | X
---+---+---
 X | X | O
---+---+---
 O | X | X
</pre><b>Draw. Best possible result against a perfect opponent.</b>
</details>
</details>
<details><summary>Play X at 7</summary><pre>
 O | O | O
---+---+---
 X | X | O
---+---+---
 X | 8 | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 8</summary><pre>
 O | O | O
---+---+---
 X | X | O
---+---+---
 7 | X | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
</details>
</details>
<details><summary>Play X at 6</summary><pre>
 O | 2 | 3
---+---+---
 O | X | X
---+---+---
 7 | 8 | 9
</pre>
O responds at 4. Your move:
<details><summary>Play X at 2</summary><pre>
 O | X | 3
---+---+---
 O | X | X
---+---+---
 O | 8 | 9
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 3</summary><pre>
 O | 2 | X
---+---+---
 O | X | X
---+---+---
 O | 8 | 9
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 7</summary><pre>
 O | 2 | O
---+---+---
 O | X | X
---+---+---
 X | 8 | 9
</pre>
O responds at 3. Your move:
<details><summary>Play X at 2</summary><pre>
 O | X | O
---+---+---
 O | X | X
---+---+---
 X | O | 9
</pre>
O responds at 8. Your move:
<details><summary>Play X at 9</summary><pre>
 O | X | O
---+---+---
 O | X | X
---+---+---
 X | O | X
</pre><b>Draw. Best possible result against a perfect opponent.</b>
</details>
</details>
<details><summary>Play X at 8</summary><pre>
 O | O | O
---+---+---
 O | X | X
---+---+---
 X | X | 9
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 9</summary><pre>
 O | O | O
---+---+---
 O | X | X
---+---+---
 X | 8 | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
</details>
<details><summary>Play X at 8</summary><pre>
 O | O | 3
---+---+---
 O | X | X
---+---+---
 7 | X | 9
</pre>
O responds at 2. Your move:
<details><summary>Play X at 3</summary><pre>
 O | O | X
---+---+---
 O | X | X
---+---+---
 O | X | 9
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 7</summary><pre>
 O | O | O
---+---+---
 O | X | X
---+---+---
 X | X | 9
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 9</summary><pre>
 O | O | O
---+---+---
 O | X | X
---+---+---
 7 | X | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
</details>
<details><summary>Play X at 9</summary><pre>
 O | 2 | O
---+---+---
 O | X | X
---+---+---
 7 | 8 | X
</pre>
O responds at 3. Your move:
<details><summary>Play X at 2</summary><pre>
 O | X | O
---+---+---
 O | X | X
---+---+---
 O | 8 | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 7</summary><pre>
 O | O | O
---+---+---
 O | X | X
---+---+---
 X | 8 | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 8</summary><pre>
 O | O | O
---+---+---
 O | X | X
---+---+---
 7 | X | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
</details>
</details>
<details><summary>Play X at 7</summary><pre>
 O | 2 | O
---+---+---
 4 | X | 6
---+---+---
 X | 8 | 9
</pre>
O responds at 3. Your move:
<details><summary>Play X at 2</summary><pre>
 O | X | O
---+---+---
 4 | X | 6
---+---+---
 X | O | 9
</pre>
O responds at 8. Your move:
<details><summary>Play X at 4</summary><pre>
 O | X | O
---+---+---
 X | X | O
---+---+---
 X | O | 9
</pre>
O responds at 6. Your move:
<details><summary>Play X at 9</summary><pre>
 O | X | O
---+---+---
 X | X | O
---+---+---
 X | O | X
</pre><b>Draw. Best possible result against a perfect opponent.</b>
</details>
</details>
<details><summary>Play X at 6</summary><pre>
 O | X | O
---+---+---
 O | X | X
---+---+---
 X | O | 9
</pre>
O responds at 4. Your move:
<details><summary>Play X at 9</summary><pre>
 O | X | O
---+---+---
 O | X | X
---+---+---
 X | O | X
</pre><b>Draw. Best possible result against a perfect opponent.</b>
</details>
</details>
<details><summary>Play X at 9</summary><pre>
 O | X | O
---+---+---
 O | X | 6
---+---+---
 X | O | X
</pre>
O responds at 4. Your move:
<details><summary>Play X at 6</summary><pre>
 O | X | O
---+---+---
 O | X | X
---+---+---
 X | O | X
</pre><b>Draw. Best possible result against a perfect opponent.</b>
</details>
</details>
</details>
<details><summary>Play X at 4</summary><pre>
 O | O | O
---+---+---
 X | X | 6
---+---+---
 X | 8 | 9
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 6</summary><pre>
 O | O | O
---+---+---
 4 | X | X
---+---+---
 X | 8 | 9
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 8</summary><pre>
 O | O | O
---+---+---
 4 | X | 6
---+---+---
 X | X | 9
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 9</summary><pre>
 O | O | O
---+---+---
 4 | X | 6
---+---+---
 X | 8 | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
</details>
<details><summary>Play X at 8</summary><pre>
 O | O | 3
---+---+---
 4 | X | 6
---+---+---
 7 | X | 9
</pre>
O responds at 2. Your move:
<details><summary>Play X at 3</summary><pre>
 O | O | X
---+---+---
 4 | X | 6
---+---+---
 O | X | 9
</pre>
O responds at 7. Your move:
<details><summary>Play X at 4</summary><pre>
 O | O | X
---+---+---
 X | X | O
---+---+---
 O | X | 9
</pre>
O responds at 6. Your move:
<details><summary>Play X at 9</summary><pre>
 O | O | X
---+---+---
 X | X | O
---+---+---
 O | X | X
</pre><b>Draw. Best possible result against a perfect opponent.</b>
</details>
</details>
<details><summary>Play X at 6</summary><pre>
 O | O | X
---+---+---
 O | X | X
---+---+---
 O | X | 9
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 9</summary><pre>
 O | O | X
---+---+---
 O | X | 6
---+---+---
 O | X | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
</details>
<details><summary>Play X at 4</summary><pre>
 O | O | O
---+---+---
 X | X | 6
---+---+---
 7 | X | 9
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 6</summary><pre>
 O | O | O
---+---+---
 4 | X | X
---+---+---
 7 | X | 9
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 7</summary><pre>
 O | O | O
---+---+---
 4 | X | 6
---+---+---
 X | X | 9
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 9</summary><pre>
 O | O | O
---+---+---
 4 | X | 6
---+---+---
 7 | X | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
</details>
<details><summary>Play X at 9</summary><pre>
 O | 2 | O
---+---+---
 4 | X | 6
---+---+---
 7 | 8 | X
</pre>
O responds at 3. Your move:
<details><summary>Play X at 2</summary><pre>
 O | X | O
---+---+---
 4 | X | 6
---+---+---
 7 | O | X
</pre>
O responds at 8. Your move:
<details><summary>Play X at 4</summary><pre>
 O | X | O
---+---+---
 X | X | O
---+---+---
 7 | O | X
</pre>
O responds at 6. Your move:
<details><summary>Play X at 7</summary><pre>
 O | X | O
---+---+---
 X | X | O
---+---+---
 X | O | X
</pre><b>Draw. Best possible result against a perfect opponent.</b>
</details>
</details>
<details><summary>Play X at 6</summary><pre>
 O | X | O
---+---+---
 O | X | X
---+---+---
 7 | O | X
</pre>
O responds at 4. Your move:
<details><summary>Play X at 7</summary><pre>
 O | X | O
---+---+---
 O | X | X
---+---+---
 X | O | X
</pre><b>Draw. Best possible result against a perfect opponent.</b>
</details>
</details>
<details><summary>Play X at 7</summary><pre>
 O | X | O
---+---+---
 O | X | 6
---+---+---
 X | O | X
</pre>
O responds at 4. Your move:
<details><summary>Play X at 6</summary><pre>
 O | X | O
---+---+---
 O | X | X
---+---+---
 X | O | X
</pre><b>Draw. Best possible result against a perfect opponent.</b>
</details>
</details>
</details>
<details><summary>Play X at 4</summary><pre>
 O | O | O
---+---+---
 X | X | 6
---+---+---
 7 | 8 | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 6</summary><pre>
 O | O | O
---+---+---
 4 | X | X
---+---+---
 7 | 8 | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 7</summary><pre>
 O | O | O
---+---+---
 4 | X | 6
---+---+---
 X | 8 | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 8</summary><pre>
 O | O | O
---+---+---
 4 | X | 6
---+---+---
 7 | X | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
</details>
</details>
<details><summary>Play X at 6</summary><pre>
 1 | 2 | O
---+---+---
 4 | 5 | X
---+---+---
 7 | 8 | 9
</pre>
O responds at 3. Your move:
<details><summary>Play X at 1</summary><pre>
 X | 2 | O
---+---+---
 O | 5 | X
---+---+---
 7 | 8 | 9
</pre>
O responds at 4. Your move:
<details><summary>Play X at 2</summary><pre>
 X | X | O
---+---+---
 O | O | X
---+---+---
 7 | 8 | 9
</pre>
O responds at 5. Your move:
<details><summary>Play X at 7</summary><pre>
 X | X | O
---+---+---
 O | O | X
---+---+---
 X | O | 9
</pre>
O responds at 8. Your move:
<details><summary>Play X at 9</summary><pre>
 X | X | O
---+---+---
 O | O | X
---+---+---
 X | O | X
</pre><b>Draw. Best possible result against a perfect opponent.</b>
</details>
</details>
<details><summary>Play X at 8</summary><pre>
 X | X | O
---+---+---
 O | O | X
---+---+---
 O | X | 9
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 9</summary><pre>
 X | X | O
---+---+---
 O | O | X
---+---+---
 O | 8 | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
</details>
<details><summary>Play X at 5</summary><pre>
 X | 2 | O
---+---+---
 O | X | X
---+---+---
 7 | 8 | O
</pre>
O responds at 9. Your move:
<details><summary>Play X at 2</summary><pre>
 X | X | O
---+---+---
 O | X | X
---+---+---
 7 | O | O
</pre>
O responds at 8. Your move:
<details><summary>Play X at 7</summary><pre>
 X | X | O
---+---+---
 O | X | X
---+---+---
 X | O | O
</pre><b>Draw. Best possible result against a perfect opponent.</b>
</details>
</details>
<details><summary>Play X at 7</summary><pre>
 X | O | O
---+---+---
 O | X | X
---+---+---
 X | 8 | O
</pre>
O responds at 2. Your move:
<details><summary>Play X at 8</summary><pre>
 X | O | O
---+---+---
 O | X | X
---+---+---
 X | X | O
</pre><b>Draw. Best possible result against a perfect opponent.</b>
</details>
</details>
<details><summary>Play X at 8</summary><pre>
 X | O | O
---+---+---
 O | X | X
---+---+---
 7 | X | O
</pre>
O responds at 2. Your move:
<details><summary>Play X at 7</summary><pre>
 X | O | O
---+---+---
 O | X | X
---+---+---
 X | X | O
</pre><b>Draw. Best possible result against a perfect opponent.</b>
</details>
</details>
</details>
<details><summary>Play X at 7</summary><pre>
 X | 2 | O
---+---+---
 O | O | X
---+---+---
 X | 8 | 9
</pre>
O responds at 5. Your move:
<details><summary>Play X at 2</summary><pre>
 X | X | O
---+---+---
 O | O | X
---+---+---
 X | O | 9
</pre>
O responds at 8. Your move:
<details><summary>Play X at 9</summary><pre>
 X | X | O
---+---+---
 O | O | X
---+---+---
 X | O | X
</pre><b>Draw. Best possible result against a perfect opponent.</b>
</details>
</details>
<details><summary>Play X at 8</summary><pre>
 X | 2 | O
---+---+---
 O | O | X
---+---+---
 X | X | O
</pre>
O responds at 9. Your move:
<details><summary>Play X at 2</summary><pre>
 X | X | O
---+---+---
 O | O | X
---+---+---
 X | X | O
</pre><b>Draw. Best possible result against a perfect opponent.</b>
</details>
</details>
<details><summary>Play X at 9</summary><pre>
 X | 2 | O
---+---+---
 O | O | X
---+---+---
 X | O | X
</pre>
O responds at 8. Your move:
<details><summary>Play X at 2</summary><pre>
 X | X | O
---+---+---
 O | O | X
---+---+---
 X | O | X
</pre><b>Draw. Best possible result against a perfect opponent.</b>
</details>
</details>
</details>
<details><summary>Play X at 8</summary><pre>
 X | 2 | O
---+---+---
 O | O | X
---+---+---
 7 | X | 9
</pre>
O responds at 5. Your move:
<details><summary>Play X at 2</summary><pre>
 X | X | O
---+---+---
 O | O | X
---+---+---
 O | X | 9
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 7</summary><pre>
 X | 2 | O
---+---+---
 O | O | X
---+---+---
 X | X | O
</pre>
O responds at 9. Your move:
<details><summary>Play X at 2</summary><pre>
 X | X | O
---+---+---
 O | O | X
---+---+---
 X | X | O
</pre><b>Draw. Best possible result against a perfect opponent.</b>
</details>
</details>
<details><summary>Play X at 9</summary><pre>
 X | 2 | O
---+---+---
 O | O | X
---+---+---
 O | X | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
</details>
<details><summary>Play X at 9</summary><pre>
 X | 2 | O
---+---+---
 O | O | X
---+---+---
 7 | 8 | X
</pre>
O responds at 5. Your move:
<details><summary>Play X at 2</summary><pre>
 X | X | O
---+---+---
 O | O | X
---+---+---
 O | 8 | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 7</summary><pre>
 X | 2 | O
---+---+---
 O | O | X
---+---+---
 X | O | X
</pre>
O responds at 8. Your move:
<details><summary>Play X at 2</summary><pre>
 X | X | O
---+---+---
 O | O | X
---+---+---
 X | O | X
</pre><b>Draw. Best possible result against a perfect opponent.</b>
</details>
</details>
<details><summary>Play X at 8</summary><pre>
 X | 2 | O
---+---+---
 O | O | X
---+---+---
 O | X | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
</details>
</details>
<details><summary>Play X at 2</summary><pre>
 1 | X | O
---+---+---
 O | 5 | X
---+---+---
 7 | 8 | 9
</pre>
O responds at 4. Your move:
<details><summary>Play X at 1</summary><pre>
 X | X | O
---+---+---
 O | O | X
---+---+---
 7 | 8 | 9
</pre>
O responds at 5. Your move:
<details><summary>Play X at 7</summary><pre>
 X | X | O
---+---+---
 O | O | X
---+---+---
 X | O | 9
</pre>
O responds at 8. Your move:
<details><summary>Play X at 9</summary><pre>
 X | X | O
---+---+---
 O | O | X
---+---+---
 X | O | X
</pre><b>Draw. Best possible result against a perfect opponent.</b>
</details>
</details>
<details><summary>Play X at 8</summary><pre>
 X | X | O
---+---+---
 O | O | X
---+---+---
 O | X | 9
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 9</summary><pre>
 X | X | O
---+---+---
 O | O | X
---+---+---
 O | 8 | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
</details>
<details><summary>Play X at 5</summary><pre>
 1 | X | O
---+---+---
 O | X | X
---+---+---
 7 | O | 9
</pre>
O responds at 8. Your move:
<details><summary>Play X at 1</summary><pre>
 X | X | O
---+---+---
 O | X | X
---+---+---
 7 | O | O
</pre>
O responds at 9. Your move:
<details><summary>Play X at 7</summary><pre>
 X | X | O
---+---+---
 O | X | X
---+---+---
 X | O | O
</pre><b>Draw. Best possible result against a perfect opponent.</b>
</details>
</details>
<details><summary>Play X at 7</summary><pre>
 O | X | O
---+---+---
 O | X | X
---+---+---
 X | O | 9
</pre>
O responds at 1. Your move:
<details><summary>Play X at 9</summary><pre>
 O | X | O
---+---+---
 O | X | X
---+---+---
 X | O | X
</pre><b>Draw. Best possible result against a perfect opponent.</b>
</details>
</details>
<details><summary>Play X at 9</summary><pre>
 O | X | O
---+---+---
 O | X | X
---+---+---
 7 | O | X
</pre>
O responds at 1. Your move:
<details><summary>Play X at 7</summary><pre>
 O | X | O
---+---+---
 O | X | X
---+---+---
 X | O | X
</pre><b>Draw. Best possible result against a perfect opponent.</b>
</details>
</details>
</details>
<details><summary>Play X at 7</summary><pre>
 1 | X | O
---+---+---
 O | O | X
---+---+---
 X | 8 | 9
</pre>
O responds at 5. Your move:
<details><summary>Play X at 1</summary><pre>
 X | X | O
---+---+---
 O | O | X
---+---+---
 X | O | 9
</pre>
O responds at 8. Your move:
<details><summary>Play X at 9</summary><pre>
 X | X | O
---+---+---
 O | O | X
---+---+---
 X | O | X
</pre><b>Draw. Best possible result against a perfect opponent.</b>
</details>
</details>
<details><summary>Play X at 8</summary><pre>
 1 | X | O
---+---+---
 O | O | X
---+---+---
 X | X | O
</pre>
O responds at 9. Your move:
<details><summary>Play X at 1</summary><pre>
 X | X | O
---+---+---
 O | O | X
---+---+---
 X | X | O
</pre><b>Draw. Best possible result against a perfect opponent.</b>
</details>
</details>
<details><summary>Play X at 9</summary><pre>
 1 | X | O
---+---+---
 O | O | X
---+---+---
 X | O | X
</pre>
O responds at 8. Your move:
<details><summary>Play X at 1</summary><pre>
 X | X | O
---+---+---
 O | O | X
---+---+---
 X | O | X
</pre><b>Draw. Best possible result against a perfect opponent.</b>
</details>
</details>
</details>
<details><summary>Play X at 8</summary><pre>
 1 | X | O
---+---+---
 O | O | X
---+---+---
 7 | X | 9
</pre>
O responds at 5. Your move:
<details><summary>Play X at 1</summary><pre>
 X | X | O
---+---+---
 O | O | X
---+---+---
 O | X | 9
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 7</summary><pre>
 1 | X | O
---+---+---
 O | O | X
---+---+---
 X | X | O
</pre>
O responds at 9. Your move:
<details><summary>Play X at 1</summary><pre>
 X | X | O
---+---+---
 O | O | X
---+---+---
 X | X | O
</pre><b>Draw. Best possible result against a perfect opponent.</b>
</details>
</details>
<details><summary>Play X at 9</summary><pre>
 1 | X | O
---+---+---
 O | O | X
---+---+---
 O | X | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
</details>
<details><summary>Play X at 9</summary><pre>
 1 | X | O
---+---+---
 O | 5 | X
---+---+---
 O | 8 | X
</pre>
O responds at 7. Your move:
<details><summary>Play X at 1</summary><pre>
 X | X | O
---+---+---
 O | O | X
---+---+---
 O | 8 | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 5</summary><pre>
 O | X | O
---+---+---
 O | X | X
---+---+---
 O | 8 | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 8</summary><pre>
 O | X | O
---+---+---
 O | 5 | X
---+---+---
 O | X | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
</details>
</details>
<details><summary>Play X at 4</summary><pre>
 1 | 2 | O
---+---+---
 X | O | X
---+---+---
 7 | 8 | 9
</pre>
O responds at 5. Your move:
<details><summary>Play X at 1</summary><pre>
 X | 2 | O
---+---+---
 X | O | X
---+---+---
 O | 8 | 9
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 2</summary><pre>
 O | X | O
---+---+---
 X | O | X
---+---+---
 7 | 8 | 9
</pre>
O responds at 1. Your move:
<details><summary>Play X at 7</summary><pre>
 O | X | O
---+---+---
 X | O | X
---+---+---
 X | 8 | O
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 8</summary><pre>
 O | X | O
---+---+---
 X | O | X
---+---+---
 O | X | 9
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 9</summary><pre>
 O | X | O
---+---+---
 X | O | X
---+---+---
 O | 8 | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
</details>
<details><summary>Play X at 7</summary><pre>
 O | 2 | O
---+---+---
 X | O | X
---+---+---
 X | 8 | 9
</pre>
O responds at 1. Your move:
<details><summary>Play X at 2</summary><pre>
 O | X | O
---+---+---
 X | O | X
---+---+---
 X | 8 | O
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 8</summary><pre>
 O | O | O
---+---+---
 X | O | X
---+---+---
 X | X | 9
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 9</summary><pre>
 O | O | O
---+---+---
 X | O | X
---+---+---
 X | 8 | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
</details>
<details><summary>Play X at 8</summary><pre>
 O | 2 | O
---+---+---
 X | O | X
---+---+---
 7 | X | 9
</pre>
O responds at 1. Your move:
<details><summary>Play X at 2</summary><pre>
 O | X | O
---+---+---
 X | O | X
---+---+---
 O | X | 9
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 7</summary><pre>
 O | O | O
---+---+---
 X | O | X
---+---+---
 X | X | 9
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 9</summary><pre>
 O | O | O
---+---+---
 X | O | X
---+---+---
 7 | X | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
</details>
<details><summary>Play X at 9</summary><pre>
 O | 2 | O
---+---+---
 X | O | X
---+---+---
 7 | 8 | X
</pre>
O responds at 1. Your move:
<details><summary>Play X at 2</summary><pre>
 O | X | O
---+---+---
 X | O | X
---+---+---
 O | 8 | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 7</summary><pre>
 O | O | O
---+---+---
 X | O | X
---+---+---
 X | 8 | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 8</summary><pre>
 O | O | O
---+---+---
 X | O | X
---+---+---
 7 | X | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
</details>
</details>
<details><summary>Play X at 5</summary><pre>
 1 | 2 | O
---+---+---
 O | X | X
---+---+---
 7 | 8 | 9
</pre>
O responds at 4. Your move:
<details><summary>Play X at 1</summary><pre>
 X | 2 | O
---+---+---
 O | X | X
---+---+---
 7 | 8 | O
</pre>
O responds at 9. Your move:
<details><summary>Play X at 2</summary><pre>
 X | X | O
---+---+---
 O | X | X
---+---+---
 7 | O | O
</pre>
O responds at 8. Your move:
<details><summary>Play X at 7</summary><pre>
 X | X | O
---+---+---
 O | X | X
---+---+---
 X | O | O
</pre><b>Draw. Best possible result against a perfect opponent.</b>
</details>
</details>
<details><summary>Play X at 7</summary><pre>
 X | O | O
---+---+---
 O | X | X
---+---+---
 X | 8 | O
</pre>
O responds at 2. Your move:
<details><summary>Play X at 8</summary><pre>
 X | O | O
---+---+---
 O | X | X
---+---+---
 X | X | O
</pre><b>Draw. Best possible result against a perfect opponent.</b>
</details>
</details>
<details><summary>Play X at 8</summary><pre>
 X | O | O
---+---+---
 O | X | X
---+---+---
 7 | X | O
</pre>
O responds at 2. Your move:
<details><summary>Play X at 7</summary><pre>
 X | O | O
---+---+---
 O | X | X
---+---+---
 X | X | O
</pre><b>Draw. Best possible result against a perfect opponent.</b>
</details>
</details>
</details>
<details><summary>Play X at 2</summary><pre>
 1 | X | O
---+---+---
 O | X | X
---+---+---
 7 | O | 9
</pre>
O responds at 8. Your move:
<details><summary>Play X at 1</summary><pre>
 X | X | O
---+---+---
 O | X | X
---+---+---
 7 | O | O
</pre>
O responds at 9. Your move:
<details><summary>Play X at 7</summary><pre>
 X | X | O
---+---+---
 O | X | X
---+---+---
 X | O | O
</pre><b>Draw. Best possible result against a perfect opponent.</b>
</details>
</details>
<details><summary>Play X at 7</summary><pre>
 O | X | O
---+---+---
 O | X | X
---+---+---
 X | O | 9
</pre>
O responds at 1. Your move:
<details><summary>Play X at 9</summary><pre>
 O | X | O
---+---+---
 O | X | X
---+---+---
 X | O | X
</pre><b>Draw. Best possible result against a perfect opponent.</b>
</details>
</details>
<details><summary>Play X at 9</summary><pre>
 O | X | O
---+---+---
 O | X | X
---+---+---
 7 | O | X
</pre>
O responds at 1. Your move:
<details><summary>Play X at 7</summary><pre>
 O | X | O
---+---+---
 O | X | X
---+---+---
 X | O | X
</pre><b>Draw. Best possible result against a perfect opponent.</b>
</details>
</details>
</details>
<details><summary>Play X at 7</summary><pre>
 O | 2 | O
---+---+---
 O | X | X
---+---+---
 X | 8 | 9
</pre>
O responds at 1. Your move:
<details><summary>Play X at 2</summary><pre>
 O | X | O
---+---+---
 O | X | X
---+---+---
 X | O | 9
</pre>
O responds at 8. Your move:
<details><summary>Play X at 9</summary><pre>
 O | X | O
---+---+---
 O | X | X
---+---+---
 X | O | X
</pre><b>Draw. Best possible result against a perfect opponent.</b>
</details>
</details>
<details><summary>Play X at 8</summary><pre>
 O | O | O
---+---+---
 O | X | X
---+---+---
 X | X | 9
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 9</summary><pre>
 O | O | O
---+---+---
 O | X | X
---+---+---
 X | 8 | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
</details>
<details><summary>Play X at 8</summary><pre>
 1 | O | O
---+---+---
 O | X | X
---+---+---
 7 | X | 9
</pre>
O responds at 2. Your move:
<details><summary>Play X at 1</summary><pre>
 X | O | O
---+---+---
 O | X | X
---+---+---
 7 | X | O
</pre>
O responds at 9. Your move:
<details><summary>Play X at 7</summary><pre>
 X | O | O
---+---+---
 O | X | X
---+---+---
 X | X | O
</pre><b>Draw. Best possible result against a perfect opponent.</b>
</details>
</details>
<details><summary>Play X at 7</summary><pre>
 O | O | O
---+---+---
 O | X | X
---+---+---
 X | X | 9
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 9</summary><pre>
 O | O | O
---+---+---
 O | X | X
---+---+---
 7 | X | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
</details>
<details><summary>Play X at 9</summary><pre>
 O | 2 | O
---+---+---
 O | X | X
---+---+---
 7 | 8 | X
</pre>
O responds at 1. Your move:
<details><summary>Play X at 2</summary><pre>
 O | X | O
---+---+---
 O | X | X
---+---+---
 O | 8 | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 7</summary><pre>
 O | O | O
---+---+---
 O | X | X
---+---+---
 X | 8 | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 8</summary><pre>
 O | O | O
---+---+---
 O | X | X
---+---+---
 7 | X | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
</details>
</details>
<details><summary>Play X at 7</summary><pre>
 O | 2 | O
---+---+---
 4 | 5 | X
---+---+---
 X | 8 | 9
</pre>
O responds at 1. Your move:
<details><summary>Play X at 2</summary><pre>
 O | X | O
---+---+---
 4 | O | X
---+---+---
 X | 8 | 9
</pre>
O responds at 5. Your move:
<details><summary>Play X at 4</summary><pre>
 O | X | O
---+---+---
 X | O | X
---+---+---
 X | 8 | O
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 8</summary><pre>
 O | X | O
---+---+---
 4 | O | X
---+---+---
 X | X | O
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 9</summary><pre>
 O | X | O
---+---+---
 4 | O | X
---+---+---
 X | O | X
</pre>
O responds at 8. Your move:
<details><summary>Play X at 4</summary><pre>
 O | X | O
---+---+---
 X | O | X
---+---+---
 X | O | X
</pre><b>Draw. Best possible result against a perfect opponent.</b>
</details>
</details>
</details>
<details><summary>Play X at 4</summary><pre>
 O | O | O
---+---+---
 X | 5 | X
---+---+---
 X | 8 | 9
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 5</summary><pre>
 O | O | O
---+---+---
 4 | X | X
---+---+---
 X | 8 | 9
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 8</summary><pre>
 O | O | O
---+---+---
 4 | 5 | X
---+---+---
 X | X | 9
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 9</summary><pre>
 O | O | O
---+---+---
 4 | 5 | X
---+---+---
 X | 8 | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
</details>
<details><summary>Play X at 8</summary><pre>
 O | 2 | O
---+---+---
 4 | 5 | X
---+---+---
 7 | X | 9
</pre>
O responds at 1. Your move:
<details><summary>Play X at 2</summary><pre>
 O | X | O
---+---+---
 4 | O | X
---+---+---
 7 | X | 9
</pre>
O responds at 5. Your move:
<details><summary>Play X at 4</summary><pre>
 O | X | O
---+---+---
 X | O | X
---+---+---
 O | X | 9
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 7</summary><pre>
 O | X | O
---+---+---
 4 | O | X
---+---+---
 X | X | O
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 9</summary><pre>
 O | X | O
---+---+---
 4 | O | X
---+---+---
 O | X | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
</details>
<details><summary>Play X at 4</summary><pre>
 O | O | O
---+---+---
 X | 5 | X
---+---+---
 7 | X | 9
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 5</summary><pre>
 O | O | O
---+---+---
 4 | X | X
---+---+---
 7 | X | 9
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 7</summary><pre>
 O | O | O
---+---+---
 4 | 5 | X
---+---+---
 X | X | 9
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 9</summary><pre>
 O | O | O
---+---+---
 4 | 5 | X
---+---+---
 7 | X | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
</details>
<details><summary>Play X at 9</summary><pre>
 O | 2 | O
---+---+---
 4 | 5 | X
---+---+---
 7 | 8 | X
</pre>
O responds at 1. Your move:
<details><summary>Play X at 2</summary><pre>
 O | X | O
---+---+---
 4 | 5 | X
---+---+---
 O | 8 | X
</pre>
O responds at 7. Your move:
<details><summary>Play X at 4</summary><pre>
 O | X | O
---+---+---
 X | O | X
---+---+---
 O | 8 | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 5</summary><pre>
 O | X | O
---+---+---
 O | X | X
---+---+---
 O | 8 | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 8</summary><pre>
 O | X | O
---+---+---
 O | 5 | X
---+---+---
 O | X | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
</details>
<details><summary>Play X at 4</summary><pre>
 O | O | O
---+---+---
 X | 5 | X
---+---+---
 7 | 8 | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 5</summary><pre>
 O | O | O
---+---+---
 4 | X | X
---+---+---
 7 | 8 | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 7</summary><pre>
 O | O | O
---+---+---
 4 | 5 | X
---+---+---
 X | 8 | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 8</summary><pre>
 O | O | O
---+---+---
 4 | 5 | X
---+---+---
 7 | X | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
</details>
</details>
<details><summary>Play X at 7</summary><pre>
 1 | 2 | 3
---+---+---
 4 | O | 6
---+---+---
 X | 8 | 9
</pre>
O responds at 5. Your move:
<details><summary>Play X at 1</summary><pre>
 X | 2 | 3
---+---+---
 O | O | 6
---+---+---
 X | 8 | 9
</pre>
O responds at 4. Your move:
<details><summary>Play X at 2</summary><pre>
 X | X | 3
---+---+---
 O | O | O
---+---+---
 X | 8 | 9
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 3</summary><pre>
 X | O | X
---+---+---
 O | O | 6
---+---+---
 X | 8 | 9
</pre>
O responds at 2. Your move:
<details><summary>Play X at 6</summary><pre>
 X | O | X
---+---+---
 O | O | X
---+---+---
 X | O | 9
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 8</summary><pre>
 X | O | X
---+---+---
 O | O | O
---+---+---
 X | X | 9
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 9</summary><pre>
 X | O | X
---+---+---
 O | O | O
---+---+---
 X | 8 | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
</details>
<details><summary>Play X at 6</summary><pre>
 X | O | 3
---+---+---
 O | O | X
---+---+---
 X | 8 | 9
</pre>
O responds at 2. Your move:
<details><summary>Play X at 3</summary><pre>
 X | O | X
---+---+---
 O | O | X
---+---+---
 X | O | 9
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 8</summary><pre>
 X | O | 3
---+---+---
 O | O | X
---+---+---
 X | X | O
</pre>
O responds at 9. Your move:
<details><summary>Play X at 3</summary><pre>
 X | O | X
---+---+---
 O | O | X
---+---+---
 X | X | O
</pre><b>Draw. Best possible result against a perfect opponent.</b>
</details>
</details>
<details><summary>Play X at 9</summary><pre>
 X | O | 3
---+---+---
 O | O | X
---+---+---
 X | O | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
</details>
<details><summary>Play X at 8</summary><pre>
 X | 2 | 3
---+---+---
 O | O | O
---+---+---
 X | X | 9
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 9</summary><pre>
 X | 2 | 3
---+---+---
 O | O | O
---+---+---
 X | 8 | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
</details>
<details><summary>Play X at 2</summary><pre>
 O | X | 3
---+---+---
 4 | O | 6
---+---+---
 X | 8 | 9
</pre>
O responds at 1. Your move:
<details><summary>Play X at 3</summary><pre>
 O | X | X
---+---+---
 O | O | 6
---+---+---
 X | 8 | 9
</pre>
O responds at 4. Your move:
<details><summary>Play X at 6</summary><pre>
 O | X | X
---+---+---
 O | O | X
---+---+---
 X | 8 | O
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 8</summary><pre>
 O | X | X
---+---+---
 O | O | O
---+---+---
 X | X | 9
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 9</summary><pre>
 O | X | X
---+---+---
 O | O | O
---+---+---
 X | 8 | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
</details>
<details><summary>Play X at 4</summary><pre>
 O | X | 3
---+---+---
 X | O | 6
---+---+---
 X | 8 | O
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 6</summary><pre>
 O | X | 3
---+---+---
 4 | O | X
---+---+---
 X | 8 | O
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 8</summary><pre>
 O | X | 3
---+---+---
 4 | O | 6
---+---+---
 X | X | O
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 9</summary><pre>
 O | X | 3
---+---+---
 4 | O | 6
---+---+---
 X | O | X
</pre>
O responds at 8. Your move:
<details><summary>Play X at 3</summary><pre>
 O | X | X
---+---+---
 4 | O | O
---+---+---
 X | O | X
</pre>
O responds at 6. Your move:
<details><summary>Play X at 4</summary><pre>
 O | X | X
---+---+---
 X | O | O
---+---+---
 X | O | X
</pre><b>Draw. Best possible result against a perfect opponent.</b>
</details>
</details>
<details><summary>Play X at 4</summary><pre>
 O | X | O
---+---+---
 X | O | 6
---+---+---
 X | O | X
</pre>
O responds at 3. Your move:
<details><summary>Play X at 6</summary><pre>
 O | X | O
---+---+---
 X | O | X
---+---+---
 X | O | X
</pre><b>Draw. Best possible result against a perfect opponent.</b>
</details>
</details>
<details><summary>Play X at 6</summary><pre>
 O | X | O
---+---+---
 4 | O | X
---+---+---
 X | O | X
</pre>
O responds at 3. Your move:
<details><summary>Play X at 4</summary><pre>
 O | X | O
---+---+---
 X | O | X
---+---+---
 X | O | X
</pre><b>Draw. Best possible result against a perfect opponent.</b>
</details>
</details>
</details>
</details>
<details><summary>Play X at 3</summary><pre>
 1 | O | X
---+---+---
 4 | O | 6
---+---+---
 X | 8 | 9
</pre>
O responds at 2. Your move:
<details><summary>Play X at 1</summary><pre>
 X | O | X
---+---+---
 O | O | 6
---+---+---
 X | 8 | 9
</pre>
O responds at 4. Your move:
<details><summary>Play X at 6</summary><pre>
 X | O | X
---+---+---
 O | O | X
---+---+---
 X | O | 9
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 8</summary><pre>
 X | O | X
---+---+---
 O | O | O
---+---+---
 X | X | 9
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 9</summary><pre>
 X | O | X
---+---+---
 O | O | O
---+---+---
 X | 8 | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
</details>
<details><summary>Play X at 4</summary><pre>
 O | O | X
---+---+---
 X | O | 6
---+---+---
 X | 8 | 9
</pre>
O responds at 1. Your move:
<details><summary>Play X at 6</summary><pre>
 O | O | X
---+---+---
 X | O | X
---+---+---
 X | O | 9
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 8</summary><pre>
 O | O | X
---+---+---
 X | O | 6
---+---+---
 X | X | O
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 9</summary><pre>
 O | O | X
---+---+---
 X | O | 6
---+---+---
 X | O | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
</details>
<details><summary>Play X at 6</summary><pre>
 1 | O | X
---+---+---
 4 | O | X
---+---+---
 X | O | 9
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 8</summary><pre>
 1 | O | X
---+---+---
 4 | O | 6
---+---+---
 X | X | O
</pre>
O responds at 9. Your move:
<details><summary>Play X at 1</summary><pre>
 X | O | X
---+---+---
 O | O | 6
---+---+---
 X | X | O
</pre>
O responds at 4. Your move:
<details><summary>Play X at 6</summary><pre>
 X | O | X
---+---+---
 O | O | X
---+---+---
 X | X | O
</pre><b>Draw. Best possible result against a perfect opponent.</b>
</details>
</details>
<details><summary>Play X at 4</summary><pre>
 O | O | X
---+---+---
 X | O | 6
---+---+---
 X | X | O
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 6</summary><pre>
 O | O | X
---+---+---
 4 | O | X
---+---+---
 X | X | O
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
</details>
<details><summary>Play X at 9</summary><pre>
 1 | O | X
---+---+---
 4 | O | 6
---+---+---
 X | O | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
</details>
<details><summary>Play X at 4</summary><pre>
 O | 2 | 3
---+---+---
 X | O | 6
---+---+---
 X | 8 | 9
</pre>
O responds at 1. Your move:
<details><summary>Play X at 2</summary><pre>
 O | X | 3
---+---+---
 X | O | 6
---+---+---
 X | 8 | O
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 3</summary><pre>
 O | O | X
---+---+---
 X | O | 6
---+---+---
 X | 8 | 9
</pre>
O responds at 2. Your move:
<details><summary>Play X at 6</summary><pre>
 O | O | X
---+---+---
 X | O | X
---+---+---
 X | O | 9
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 8</summary><pre>
 O | O | X
---+---+---
 X | O | 6
---+---+---
 X | X | O
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 9</summary><pre>
 O | O | X
---+---+---
 X | O | 6
---+---+---
 X | O | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
</details>
<details><summary>Play X at 6</summary><pre>
 O | O | 3
---+---+---
 X | O | X
---+---+---
 X | 8 | 9
</pre>
O responds at 2. Your move:
<details><summary>Play X at 3</summary><pre>
 O | O | X
---+---+---
 X | O | X
---+---+---
 X | O | 9
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 8</summary><pre>
 O | O | O
---+---+---
 X | O | X
---+---+---
 X | X | 9
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 9</summary><pre>
 O | O | O
---+---+---
 X | O | X
---+---+---
 X | 8 | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
</details>
<details><summary>Play X at 8</summary><pre>
 O | 2 | 3
---+---+---
 X | O | 6
---+---+---
 X | X | O
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 9</summary><pre>
 O | 2 | 3
---+---+---
 X | O | 6
---+---+---
 X | O | X
</pre>
O responds at 8. Your move:
<details><summary>Play X at 2</summary><pre>
 O | X | O
---+---+---
 X | O | 6
---+---+---
 X | O | X
</pre>
O responds at 3. Your move:
<details><summary>Play X at 6</summary><pre>
 O | X | O
---+---+---
 X | O | X
---+---+---
 X | O | X
</pre><b>Draw. Best possible result against a perfect opponent.</b>
</details>
</details>
<details><summary>Play X at 3</summary><pre>
 O | O | X
---+---+---
 X | O | 6
---+---+---
 X | O | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 6</summary><pre>
 O | O | 3
---+---+---
 X | O | X
---+---+---
 X | O | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
</details>
</details>
<details><summary>Play X at 6</summary><pre>
 1 | O | 3
---+---+---
 4 | O | X
---+---+---
 X | 8 | 9
</pre>
O responds at 2. Your move:
<details><summary>Play X at 1</summary><pre>
 X | O | 3
---+---+---
 4 | O | X
---+---+---
 X | O | 9
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 3</summary><pre>
 1 | O | X
---+---+---
 4 | O | X
---+---+---
 X | O | 9
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 4</summary><pre>
 O | O | 3
---+---+---
 X | O | X
---+---+---
 X | 8 | 9
</pre>
O responds at 1. Your move:
<details><summary>Play X at 3</summary><pre>
 O | O | X
---+---+---
 X | O | X
---+---+---
 X | O | 9
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 8</summary><pre>
 O | O | O
---+---+---
 X | O | X
---+---+---
 X | X | 9
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 9</summary><pre>
 O | O | O
---+---+---
 X | O | X
---+---+---
 X | 8 | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
</details>
<details><summary>Play X at 8</summary><pre>
 1 | O | 3
---+---+---
 4 | O | X
---+---+---
 X | X | O
</pre>
O responds at 9. Your move:
<details><summary>Play X at 1</summary><pre>
 X | O | 3
---+---+---
 O | O | X
---+---+---
 X | X | O
</pre>
O responds at 4. Your move:
<details><summary>Play X at 3</summary><pre>
 X | O | X
---+---+---
 O | O | X
---+---+---
 X | X | O
</pre><b>Draw. Best possible result against a perfect opponent.</b>
</details>
</details>
<details><summary>Play X at 3</summary><pre>
 O | O | X
---+---+---
 4 | O | X
---+---+---
 X | X | O
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 4</summary><pre>
 O | O | 3
---+---+---
 X | O | X
---+---+---
 X | X | O
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
</details>
<details><summary>Play X at 9</summary><pre>
 1 | O | 3
---+---+---
 4 | O | X
---+---+---
 X | O | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
</details>
<details><summary>Play X at 8</summary><pre>
 1 | 2 | 3
---+---+---
 4 | O | 6
---+---+---
 X | X | O
</pre>
O responds at 9. Your move:
<details><summary>Play X at 1</summary><pre>
 X | 2 | 3
---+---+---
 O | O | 6
---+---+---
 X | X | O
</pre>
O responds at 4. Your move:
<details><summary>Play X at 2</summary><pre>
 X | X | 3
---+---+---
 O | O | O
---+---+---
 X | X | O
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 3</summary><pre>
 X | 2 | X
---+---+---
 O | O | O
---+---+---
 X | X | O
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 6</summary><pre>
 X | O | 3
---+---+---
 O | O | X
---+---+---
 X | X | O
</pre>
O responds at 2. Your move:
<details><summary>Play X at 3</summary><pre>
 X | O | X
---+---+---
 O | O | X
---+---+---
 X | X | O
</pre><b>Draw. Best possible result against a perfect opponent.</b>
</details>
</details>
</details>
<details><summary>Play X at 2</summary><pre>
 O | X | 3
---+---+---
 4 | O | 6
---+---+---
 X | X | O
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 3</summary><pre>
 O | 2 | X
---+---+---
 4 | O | 6
---+---+---
 X | X | O
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 4</summary><pre>
 O | 2 | 3
---+---+---
 X | O | 6
---+---+---
 X | X | O
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 6</summary><pre>
 O | 2 | 3
---+---+---
 4 | O | X
---+---+---
 X | X | O
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
</details>
<details><summary>Play X at 9</summary><pre>
 1 | 2 | 3
---+---+---
 4 | O | 6
---+---+---
 X | O | X
</pre>
O responds at 8. Your move:
<details><summary>Play X at 1</summary><pre>
 X | O | 3
---+---+---
 4 | O | 6
---+---+---
 X | O | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 2</summary><pre>
 O | X | 3
---+---+---
 4 | O | 6
---+---+---
 X | O | X
</pre>
O responds at 1. Your move:
<details><summary>Play X at 3</summary><pre>
 O | X | X
---+---+---
 4 | O | O
---+---+---
 X | O | X
</pre>
O responds at 6. Your move:
<details><summary>Play X at 4</summary><pre>
 O | X | X
---+---+---
 X | O | O
---+---+---
 X | O | X
</pre><b>Draw. Best possible result against a perfect opponent.</b>
</details>
</details>
<details><summary>Play X at 4</summary><pre>
 O | X | O
---+---+---
 X | O | 6
---+---+---
 X | O | X
</pre>
O responds at 3. Your move:
<details><summary>Play X at 6</summary><pre>
 O | X | O
---+---+---
 X | O | X
---+---+---
 X | O | X
</pre><b>Draw. Best possible result against a perfect opponent.</b>
</details>
</details>
<details><summary>Play X at 6</summary><pre>
 O | X | O
---+---+---
 4 | O | X
---+---+---
 X | O | X
</pre>
O responds at 3. Your move:
<details><summary>Play X at 4</summary><pre>
 O | X | O
---+---+---
 X | O | X
---+---+---
 X | O | X
</pre><b>Draw. Best possible result against a perfect opponent.</b>
</details>
</details>
</details>
<details><summary>Play X at 3</summary><pre>
 1 | O | X
---+---+---
 4 | O | 6
---+---+---
 X | O | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 4</summary><pre>
 1 | O | 3
---+---+---
 X | O | 6
---+---+---
 X | O | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 6</summary><pre>
 1 | O | 3
---+---+---
 4 | O | X
---+---+---
 X | O | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
</details>
</details>
<details><summary>Play X at 8</summary><pre>
 1 | O | 3
---+---+---
 4 | 5 | 6
---+---+---
 7 | X | 9
</pre>
O responds at 2. Your move:
<details><summary>Play X at 1</summary><pre>
 X | O | 3
---+---+---
 4 | 5 | 6
---+---+---
 O | X | 9
</pre>
O responds at 7. Your move:
<details><summary>Play X at 3</summary><pre>
 X | O | X
---+---+---
 4 | O | 6
---+---+---
 O | X | 9
</pre>
O responds at 5. Your move:
<details><summary>Play X at 4</summary><pre>
 X | O | X
---+---+---
 X | O | O
---+---+---
 O | X | 9
</pre>
O responds at 6. Your move:
<details><summary>Play X at 9</summary><pre>
 X | O | X
---+---+---
 X | O | O
---+---+---
 O | X | X
</pre><b>Draw. Best possible result against a perfect opponent.</b>
</details>
</details>
<details><summary>Play X at 6</summary><pre>
 X | O | X
---+---+---
 4 | O | X
---+---+---
 O | X | O
</pre>
O responds at 9. Your move:
<details><summary>Play X at 4</summary><pre>
 X | O | X
---+---+---
 X | O | X
---+---+---
 O | X | O
</pre><b>Draw. Best possible result against a perfect opponent.</b>
</details>
</details>
<details><summary>Play X at 9</summary><pre>
 X | O | X
---+---+---
 4 | O | O
---+---+---
 O | X | X
</pre>
O responds at 6. Your move:
<details><summary>Play X at 4</summary><pre>
 X | O | X
---+---+---
 X | O | O
---+---+---
 O | X | X
</pre><b>Draw. Best possible result against a perfect opponent.</b>
</details>
</details>
</details>
<details><summary>Play X at 4</summary><pre>
 X | O | 3
---+---+---
 X | O | 6
---+---+---
 O | X | 9
</pre>
O responds at 5. Your move:
<details><summary>Play X at 3</summary><pre>
 X | O | X
---+---+---
 X | O | O
---+---+---
 O | X | 9
</pre>
O responds at 6. Your move:
<details><summary>Play X at 9</summary><pre>
 X | O | X
---+---+---
 X | O | O
---+---+---
 O | X | X
</pre><b>Draw. Best possible result against a perfect opponent.</b>
</details>
</details>
<details><summary>Play X at 6</summary><pre>
 X | O | O
---+---+---
 X | O | X
---+---+---
 O | X | 9
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 9</summary><pre>
 X | O | O
---+---+---
 X | O | 6
---+---+---
 O | X | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
</details>
<details><summary>Play X at 5</summary><pre>
 X | O | 3
---+---+---
 4 | X | 6
---+---+---
 O | X | O
</pre>
O responds at 9. Your move:
<details><summary>Play X at 3</summary><pre>
 X | O | X
---+---+---
 O | X | 6
---+---+---
 O | X | O
</pre>
O responds at 4. Your move:
<details><summary>Play X at 6</summary><pre>
 X | O | X
---+---+---
 O | X | X
---+---+---
 O | X | O
</pre><b>Draw. Best possible result against a perfect opponent.</b>
</details>
</details>
<details><summary>Play X at 4</summary><pre>
 X | O | 3
---+---+---
 X | X | O
---+---+---
 O | X | O
</pre>
O responds at 6. Your move:
<details><summary>Play X at 3</summary><pre>
 X | O | X
---+---+---
 X | X | O
---+---+---
 O | X | O
</pre><b>Draw. Best possible result against a perfect opponent.</b>
</details>
</details>
<details><summary>Play X at 6</summary><pre>
 X | O | 3
---+---+---
 O | X | X
---+---+---
 O | X | O
</pre>
O responds at 4. Your move:
<details><summary>Play X at 3</summary><pre>
 X | O | X
---+---+---
 O | X | X
---+---+---
 O | X | O
</pre><b>Draw. Best possible result against a perfect opponent.</b>
</details>
</details>
</details>
<details><summary>Play X at 6</summary><pre>
 X | O | 3
---+---+---
 4 | O | X
---+---+---
 O | X | 9
</pre>
O responds at 5. Your move:
<details><summary>Play X at 3</summary><pre>
 X | O | X
---+---+---
 4 | O | X
---+---+---
 O | X | O
</pre>
O responds at 9. Your move:
<details><summary>Play X at 4</summary><pre>
 X | O | X
---+---+---
 X | O | X
---+---+---
 O | X | O
</pre><b>Draw. Best possible result against a perfect opponent.</b>
</details>
</details>
<details><summary>Play X at 4</summary><pre>
 X | O | O
---+---+---
 X | O | X
---+---+---
 O | X | 9
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 9</summary><pre>
 X | O | O
---+---+---
 4 | O | X
---+---+---
 O | X | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
</details>
<details><summary>Play X at 9</summary><pre>
 X | O | 3
---+---+---
 4 | O | 6
---+---+---
 O | X | X
</pre>
O responds at 5. Your move:
<details><summary>Play X at 3</summary><pre>
 X | O | X
---+---+---
 4 | O | O
---+---+---
 O | X | X
</pre>
O responds at 6. Your move:
<details><summary>Play X at 4</summary><pre>
 X | O | X
---+---+---
 X | O | O
---+---+---
 O | X | X
</pre><b>Draw. Best possible result against a perfect opponent.</b>
</details>
</details>
<details><summary>Play X at 4</summary><pre>
 X | O | O
---+---+---
 X | O | 6
---+---+---
 O | X | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 6</summary><pre>
 X | O | O
---+---+---
 4 | O | X
---+---+---
 O | X | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
</details>
</details>
<details><summary>Play X at 3</summary><pre>
 1 | O | X
---+---+---
 4 | 5 | 6
---+---+---
 O | X | 9
</pre>
O responds at 7. Your move:
<details><summary>Play X at 1</summary><pre>
 X | O | X
---+---+---
 4 | O | 6
---+---+---
 O | X | 9
</pre>
O responds at 5. Your move:
<details><summary>Play X at 4</summary><pre>
 X | O | X
---+---+---
 X | O | O
---+---+---
 O | X | 9
</pre>
O responds at 6. Your move:
<details><summary>Play X at 9</summary><pre>
 X | O | X
---+---+---
 X | O | O
---+---+---
 O | X | X
</pre><b>Draw. Best possible result against a perfect opponent.</b>
</details>
</details>
<details><summary>Play X at 6</summary><pre>
 X | O | X
---+---+---
 4 | O | X
---+---+---
 O | X | O
</pre>
O responds at 9. Your move:
<details><summary>Play X at 4</summary><pre>
 X | O | X
---+---+---
 X | O | X
---+---+---
 O | X | O
</pre><b>Draw. Best possible result against a perfect opponent.</b>
</details>
</details>
<details><summary>Play X at 9</summary><pre>
 X | O | X
---+---+---
 4 | O | O
---+---+---
 O | X | X
</pre>
O responds at 6. Your move:
<details><summary>Play X at 4</summary><pre>
 X | O | X
---+---+---
 X | O | O
---+---+---
 O | X | X
</pre><b>Draw. Best possible result against a perfect opponent.</b>
</details>
</details>
</details>
<details><summary>Play X at 4</summary><pre>
 1 | O | X
---+---+---
 X | O | 6
---+---+---
 O | X | 9
</pre>
O responds at 5. Your move:
<details><summary>Play X at 1</summary><pre>
 X | O | X
---+---+---
 X | O | O
---+---+---
 O | X | 9
</pre>
O responds at 6. Your move:
<details><summary>Play X at 9</summary><pre>
 X | O | X
---+---+---
 X | O | O
---+---+---
 O | X | X
</pre><b>Draw. Best possible result against a perfect opponent.</b>
</details>
</details>
<details><summary>Play X at 6</summary><pre>
 1 | O | X
---+---+---
 X | O | X
---+---+---
 O | X | O
</pre>
O responds at 9. Your move:
<details><summary>Play X at 1</summary><pre>
 X | O | X
---+---+---
 X | O | X
---+---+---
 O | X | O
</pre><b>Draw. Best possible result against a perfect opponent.</b>
</details>
</details>
<details><summary>Play X at 9</summary><pre>
 1 | O | X
---+---+---
 X | O | O
---+---+---
 O | X | X
</pre>
O responds at 6. Your move:
<details><summary>Play X at 1</summary><pre>
 X | O | X
---+---+---
 X | O | O
---+---+---
 O | X | X
</pre><b>Draw. Best possible result against a perfect opponent.</b>
</details>
</details>
</details>
<details><summary>Play X at 5</summary><pre>
 O | O | X
---+---+---
 4 | X | 6
---+---+---
 O | X | 9
</pre>
O responds at 1. Your move:
<details><summary>Play X at 4</summary><pre>
 O | O | X
---+---+---
 X | X | O
---+---+---
 O | X | 9
</pre>
O responds at 6. Your move:
<details><summary>Play X at 9</summary><pre>
 O | O | X
---+---+---
 X | X | O
---+---+---
 O | X | X
</pre><b>Draw. Best possible result against a perfect opponent.</b>
</details>
</details>
<details><summary>Play X at 6</summary><pre>
 O | O | X
---+---+---
 O | X | X
---+---+---
 O | X | 9
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 9</summary><pre>
 O | O | X
---+---+---
 O | X | 6
---+---+---
 O | X | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
</details>
<details><summary>Play X at 6</summary><pre>
 1 | O | X
---+---+---
 4 | 5 | X
---+---+---
 O | X | O
</pre>
O responds at 9. Your move:
<details><summary>Play X at 1</summary><pre>
 X | O | X
---+---+---
 O | 5 | X
---+---+---
 O | X | O
</pre>
O responds at 4. Your move:
<details><summary>Play X at 5</summary><pre>
 X | O | X
---+---+---
 O | X | X
---+---+---
 O | X | O
</pre><b>Draw. Best possible result against a perfect opponent.</b>
</details>
</details>
<details><summary>Play X at 4</summary><pre>
 1 | O | X
---+---+---
 X | O | X
---+---+---
 O | X | O
</pre>
O responds at 5. Your move:
<details><summary>Play X at 1</summary><pre>
 X | O | X
---+---+---
 X | O | X
---+---+---
 O | X | O
</pre><b>Draw. Best possible result against a perfect opponent.</b>
</details>
</details>
<details><summary>Play X at 5</summary><pre>
 1 | O | X
---+---+---
 O | X | X
---+---+---
 O | X | O
</pre>
O responds at 4. Your move:
<details><summary>Play X at 1</summary><pre>
 X | O | X
---+---+---
 O | X | X
---+---+---
 O | X | O
</pre><b>Draw. Best possible result against a perfect opponent.</b>
</details>
</details>
</details>
<details><summary>Play X at 9</summary><pre>
 1 | O | X
---+---+---
 4 | 5 | O
---+---+---
 O | X | X
</pre>
O responds at 6. Your move:
<details><summary>Play X at 1</summary><pre>
 X | O | X
---+---+---
 4 | O | O
---+---+---
 O | X | X
</pre>
O responds at 5. Your move:
<details><summary>Play X at 4</summary><pre>
 X | O | X
---+---+---
 X | O | O
---+---+---
 O | X | X
</pre><b>Draw. Best possible result against a perfect opponent.</b>
</details>
</details>
<details><summary>Play X at 4</summary><pre>
 O | O | X
---+---+---
 X | 5 | O
---+---+---
 O | X | X
</pre>
O responds at 1. Your move:
<details><summary>Play X at 5</summary><pre>
 O | O | X
---+---+---
 X | X | O
---+---+---
 O | X | X
</pre><b>Draw. Best possible result against a perfect opponent.</b>
</details>
</details>
<details><summary>Play X at 5</summary><pre>
 O | O | X
---+---+---
 4 | X | O
---+---+---
 O | X | X
</pre>
O responds at 1. Your move:
<details><summary>Play X at 4</summary><pre>
 O | O | X
---+---+---
 X | X | O
---+---+---
 O | X | X
</pre><b>Draw. Best possible result against a perfect opponent.</b>
</details>
</details>
</details>
</details>
<details><summary>Play X at 4</summary><pre>
 1 | O | 3
---+---+---
 X | 5 | 6
---+---+---
 O | X | 9
</pre>
O responds at 7. Your move:
<details><summary>Play X at 1</summary><pre>
 X | O | 3
---+---+---
 X | O | 6
---+---+---
 O | X | 9
</pre>
O responds at 5. Your move:
<details><summary>Play X at 3</summary><pre>
 X | O | X
---+---+---
 X | O | O
---+---+---
 O | X | 9
</pre>
O responds at 6. Your move:
<details><summary>Play X at 9</summary><pre>
 X | O | X
---+---+---
 X | O | O
---+---+---
 O | X | X
</pre><b>Draw. Best possible result against a perfect opponent.</b>
</details>
</details>
<details><summary>Play X at 6</summary><pre>
 X | O | O
---+---+---
 X | O | X
---+---+---
 O | X | 9
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 9</summary><pre>
 X | O | O
---+---+---
 X | O | 6
---+---+---
 O | X | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
</details>
<details><summary>Play X at 3</summary><pre>
 1 | O | X
---+---+---
 X | O | 6
---+---+---
 O | X | 9
</pre>
O responds at 5. Your move:
<details><summary>Play X at 1</summary><pre>
 X | O | X
---+---+---
 X | O | O
---+---+---
 O | X | 9
</pre>
O responds at 6. Your move:
<details><summary>Play X at 9</summary><pre>
 X | O | X
---+---+---
 X | O | O
---+---+---
 O | X | X
</pre><b>Draw. Best possible result against a perfect opponent.</b>
</details>
</details>
<details><summary>Play X at 6</summary><pre>
 1 | O | X
---+---+---
 X | O | X
---+---+---
 O | X | O
</pre>
O responds at 9. Your move:
<details><summary>Play X at 1</summary><pre>
 X | O | X
---+---+---
 X | O | X
---+---+---
 O | X | O
</pre><b>Draw. Best possible result against a perfect opponent.</b>
</details>
</details>
<details><summary>Play X at 9</summary><pre>
 1 | O | X
---+---+---
 X | O | O
---+---+---
 O | X | X
</pre>
O responds at 6. Your move:
<details><summary>Play X at 1</summary><pre>
 X | O | X
---+---+---
 X | O | O
---+---+---
 O | X | X
</pre><b>Draw. Best possible result against a perfect opponent.</b>
</details>
</details>
</details>
<details><summary>Play X at 5</summary><pre>
 1 | O | 3
---+---+---
 X | X | O
---+---+---
 O | X | 9
</pre>
O responds at 6. Your move:
<details><summary>Play X at 1</summary><pre>
 X | O | 3
---+---+---
 X | X | O
---+---+---
 O | X | O
</pre>
O responds at 9. Your move:
<details><summary>Play X at 3</summary><pre>
 X | O | X
---+---+---
 X | X | O
---+---+---
 O | X | O
</pre><b>Draw. Best possible result against a perfect opponent.</b>
</details>
</details>
<details><summary>Play X at 3</summary><pre>
 O | O | X
---+---+---
 X | X | O
---+---+---
 O | X | 9
</pre>
O responds at 1. Your move:
<details><summary>Play X at 9</summary><pre>
 O | O | X
---+---+---
 X | X | O
---+---+---
 O | X | X
</pre><b>Draw. Best possible result against a perfect opponent.</b>
</details>
</details>
<details><summary>Play X at 9</summary><pre>
 O | O | 3
---+---+---
 X | X | O
---+---+---
 O | X | X
</pre>
O responds at 1. Your move:
<details><summary>Play X at 3</summary><pre>
 O | O | X
---+---+---
 X | X | O
---+---+---
 O | X | X
</pre><b>Draw. Best possible result against a perfect opponent.</b>
</details>
</details>
</details>
<details><summary>Play X at 6</summary><pre>
 1 | O | 3
---+---+---
 X | O | X
---+---+---
 O | X | 9
</pre>
O responds at 5. Your move:
<details><summary>Play X at 1</summary><pre>
 X | O | O
---+---+---
 X | O | X
---+---+---
 O | X | 9
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 3</summary><pre>
 1 | O | X
---+---+---
 X | O | X
---+---+---
 O | X | O
</pre>
O responds at 9. Your move:
<details><summary>Play X at 1</summary><pre>
 X | O | X
---+---+---
 X | O | X
---+---+---
 O | X | O
</pre><b>Draw. Best possible result against a perfect opponent.</b>
</details>
</details>
<details><summary>Play X at 9</summary><pre>
 1 | O | O
---+---+---
 X | O | X
---+---+---
 O | X | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
</details>
<details><summary>Play X at 9</summary><pre>
 1 | O | O
---+---+---
 X | 5 | 6
---+---+---
 O | X | X
</pre>
O responds at 3. Your move:
<details><summary>Play X at 1</summary><pre>
 X | O | O
---+---+---
 X | O | 6
---+---+---
 O | X | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 5</summary><pre>
 O | O | O
---+---+---
 X | X | 6
---+---+---
 O | X | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 6</summary><pre>
 O | O | O
---+---+---
 X | 5 | X
---+---+---
 O | X | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
</details>
</details>
<details><summary>Play X at 5</summary><pre>
 O | O | 3
---+---+---
 4 | X | 6
---+---+---
 7 | X | 9
</pre>
O responds at 1. Your move:
<details><summary>Play X at 3</summary><pre>
 O | O | X
---+---+---
 4 | X | 6
---+---+---
 O | X | 9
</pre>
O responds at 7. Your move:
<details><summary>Play X at 4</summary><pre>
 O | O | X
---+---+---
 X | X | O
---+---+---
 O | X | 9
</pre>
O responds at 6. Your move:
<details><summary>Play X at 9</summary><pre>
 O | O | X
---+---+---
 X | X | O
---+---+---
 O | X | X
</pre><b>Draw. Best possible result against a perfect opponent.</b>
</details>
</details>
<details><summary>Play X at 6</summary><pre>
 O | O | X
---+---+---
 O | X | X
---+---+---
 O | X | 9
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 9</summary><pre>
 O | O | X
---+---+---
 O | X | 6
---+---+---
 O | X | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
</details>
<details><summary>Play X at 4</summary><pre>
 O | O | O
---+---+---
 X | X | 6
---+---+---
 7 | X | 9
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 6</summary><pre>
 O | O | O
---+---+---
 4 | X | X
---+---+---
 7 | X | 9
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 7</summary><pre>
 O | O | O
---+---+---
 4 | X | 6
---+---+---
 X | X | 9
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 9</summary><pre>
 O | O | O
---+---+---
 4 | X | 6
---+---+---
 7 | X | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
</details>
<details><summary>Play X at 6</summary><pre>
 1 | O | 3
---+---+---
 4 | 5 | X
---+---+---
 O | X | 9
</pre>
O responds at 7. Your move:
<details><summary>Play X at 1</summary><pre>
 X | O | 3
---+---+---
 4 | O | X
---+---+---
 O | X | 9
</pre>
O responds at 5. Your move:
<details><summary>Play X at 3</summary><pre>
 X | O | X
---+---+---
 4 | O | X
---+---+---
 O | X | O
</pre>
O responds at 9. Your move:
<details><summary>Play X at 4</summary><pre>
 X | O | X
---+---+---
 X | O | X
---+---+---
 O | X | O
</pre><b>Draw. Best possible result against a perfect opponent.</b>
</details>
</details>
<details><summary>Play X at 4</summary><pre>
 X | O | O
---+---+---
 X | O | X
---+---+---
 O | X | 9
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 9</summary><pre>
 X | O | O
---+---+---
 4 | O | X
---+---+---
 O | X | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
</details>
<details><summary>Play X at 3</summary><pre>
 1 | O | X
---+---+---
 4 | 5 | X
---+---+---
 O | X | O
</pre>
O responds at 9. Your move:
<details><summary>Play X at 1</summary><pre>
 X | O | X
---+---+---
 O | 5 | X
---+---+---
 O | X | O
</pre>
O responds at 4. Your move:
<details><summary>Play X at 5</summary><pre>
 X | O | X
---+---+---
 O | X | X
---+---+---
 O | X | O
</pre><b>Draw. Best possible result against a perfect opponent.</b>
</details>
</details>
<details><summary>Play X at 4</summary><pre>
 1 | O | X
---+---+---
 X | O | X
---+---+---
 O | X | O
</pre>
O responds at 5. Your move:
<details><summary>Play X at 1</summary><pre>
 X | O | X
---+---+---
 X | O | X
---+---+---
 O | X | O
</pre><b>Draw. Best possible result against a perfect opponent.</b>
</details>
</details>
<details><summary>Play X at 5</summary><pre>
 1 | O | X
---+---+---
 O | X | X
---+---+---
 O | X | O
</pre>
O responds at 4. Your move:
<details><summary>Play X at 1</summary><pre>
 X | O | X
---+---+---
 O | X | X
---+---+---
 O | X | O
</pre><b>Draw. Best possible result against a perfect opponent.</b>
</details>
</details>
</details>
<details><summary>Play X at 4</summary><pre>
 1 | O | 3
---+---+---
 X | O | X
---+---+---
 O | X | 9
</pre>
O responds at 5. Your move:
<details><summary>Play X at 1</summary><pre>
 X | O | O
---+---+---
 X | O | X
---+---+---
 O | X | 9
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 3</summary><pre>
 1 | O | X
---+---+---
 X | O | X
---+---+---
 O | X | O
</pre>
O responds at 9. Your move:
<details><summary>Play X at 1</summary><pre>
 X | O | X
---+---+---
 X | O | X
---+---+---
 O | X | O
</pre><b>Draw. Best possible result against a perfect opponent.</b>
</details>
</details>
<details><summary>Play X at 9</summary><pre>
 1 | O | O
---+---+---
 X | O | X
---+---+---
 O | X | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
</details>
<details><summary>Play X at 5</summary><pre>
 1 | O | 3
---+---+---
 O | X | X
---+---+---
 O | X | 9
</pre>
O responds at 4. Your move:
<details><summary>Play X at 1</summary><pre>
 X | O | 3
---+---+---
 O | X | X
---+---+---
 O | X | O
</pre>
O responds at 9. Your move:
<details><summary>Play X at 3</summary><pre>
 X | O | X
---+---+---
 O | X | X
---+---+---
 O | X | O
</pre><b>Draw. Best possible result against a perfect opponent.</b>
</details>
</details>
<details><summary>Play X at 3</summary><pre>
 O | O | X
---+---+---
 O | X | X
---+---+---
 O | X | 9
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 9</summary><pre>
 O | O | 3
---+---+---
 O | X | X
---+---+---
 O | X | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
</details>
<details><summary>Play X at 9</summary><pre>
 1 | O | O
---+---+---
 4 | 5 | X
---+---+---
 O | X | X
</pre>
O responds at 3. Your move:
<details><summary>Play X at 1</summary><pre>
 X | O | O
---+---+---
 4 | O | X
---+---+---
 O | X | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 4</summary><pre>
 O | O | O
---+---+---
 X | 5 | X
---+---+---
 O | X | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 5</summary><pre>
 O | O | O
---+---+---
 4 | X | X
---+---+---
 O | X | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
</details>
</details>
<details><summary>Play X at 7</summary><pre>
 1 | O | 3
---+---+---
 4 | 5 | 6
---+---+---
 X | X | O
</pre>
O responds at 9. Your move:
<details><summary>Play X at 1</summary><pre>
 X | O | 3
---+---+---
 O | 5 | 6
---+---+---
 X | X | O
</pre>
O responds at 4. Your move:
<details><summary>Play X at 3</summary><pre>
 X | O | X
---+---+---
 O | O | 6
---+---+---
 X | X | O
</pre>
O responds at 5. Your move:
<details><summary>Play X at 6</summary><pre>
 X | O | X
---+---+---
 O | O | X
---+---+---
 X | X | O
</pre><b>Draw. Best possible result against a perfect opponent.</b>
</details>
</details>
<details><summary>Play X at 5</summary><pre>
 X | O | O
---+---+---
 O | X | 6
---+---+---
 X | X | O
</pre>
O responds at 3. Your move:
<details><summary>Play X at 6</summary><pre>
 X | O | O
---+---+---
 O | X | X
---+---+---
 X | X | O
</pre><b>Draw. Best possible result against a perfect opponent.</b>
</details>
</details>
<details><summary>Play X at 6</summary><pre>
 X | O | O
---+---+---
 O | 5 | X
---+---+---
 X | X | O
</pre>
O responds at 3. Your move:
<details><summary>Play X at 5</summary><pre>
 X | O | O
---+---+---
 O | X | X
---+---+---
 X | X | O
</pre><b>Draw. Best possible result against a perfect opponent.</b>
</details>
</details>
</details>
<details><summary>Play X at 3</summary><pre>
 1 | O | X
---+---+---
 4 | O | 6
---+---+---
 X | X | O
</pre>
O responds at 5. Your move:
<details><summary>Play X at 1</summary><pre>
 X | O | X
---+---+---
 O | O | 6
---+---+---
 X | X | O
</pre>
O responds at 4. Your move:
<details><summary>Play X at 6</summary><pre>
 X | O | X
---+---+---
 O | O | X
---+---+---
 X | X | O
</pre><b>Draw. Best possible result against a perfect opponent.</b>
</details>
</details>
<details><summary>Play X at 4</summary><pre>
 O | O | X
---+---+---
 X | O | 6
---+---+---
 X | X | O
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 6</summary><pre>
 O | O | X
---+---+---
 4 | O | X
---+---+---
 X | X | O
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
</details>
<details><summary>Play X at 4</summary><pre>
 O | O | 3
---+---+---
 X | 5 | 6
---+---+---
 X | X | O
</pre>
O responds at 1. Your move:
<details><summary>Play X at 3</summary><pre>
 O | O | X
---+---+---
 X | O | 6
---+---+---
 X | X | O
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 5</summary><pre>
 O | O | O
---+---+---
 X | X | 6
---+---+---
 X | X | O
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 6</summary><pre>
 O | O | O
---+---+---
 X | 5 | X
---+---+---
 X | X | O
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
</details>
<details><summary>Play X at 5</summary><pre>
 1 | O | O
---+---+---
 4 | X | 6
---+---+---
 X | X | O
</pre>
O responds at 3. Your move:
<details><summary>Play X at 1</summary><pre>
 X | O | O
---+---+---
 4 | X | O
---+---+---
 X | X | O
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 4</summary><pre>
 O | O | O
---+---+---
 X | X | 6
---+---+---
 X | X | O
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 6</summary><pre>
 O | O | O
---+---+---
 4 | X | X
---+---+---
 X | X | O
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
</details>
<details><summary>Play X at 6</summary><pre>
 O | O | 3
---+---+---
 4 | 5 | X
---+---+---
 X | X | O
</pre>
O responds at 1. Your move:
<details><summary>Play X at 3</summary><pre>
 O | O | X
---+---+---
 4 | O | X
---+---+---
 X | X | O
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 4</summary><pre>
 O | O | O
---+---+---
 X | 5 | X
---+---+---
 X | X | O
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 5</summary><pre>
 O | O | O
---+---+---
 4 | X | X
---+---+---
 X | X | O
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
</details>
</details>
<details><summary>Play X at 9</summary><pre>
 1 | O | 3
---+---+---
 4 | 5 | 6
---+---+---
 O | X | X
</pre>
O responds at 7. Your move:
<details><summary>Play X at 1</summary><pre>
 X | O | 3
---+---+---
 4 | O | 6
---+---+---
 O | X | X
</pre>
O responds at 5. Your move:
<details><summary>Play X at 3</summary><pre>
 X | O | X
---+---+---
 4 | O | O
---+---+---
 O | X | X
</pre>
O responds at 6. Your move:
<details><summary>Play X at 4</summary><pre>
 X | O | X
---+---+---
 X | O | O
---+---+---
 O | X | X
</pre><b>Draw. Best possible result against a perfect opponent.</b>
</details>
</details>
<details><summary>Play X at 4</summary><pre>
 X | O | O
---+---+---
 X | O | 6
---+---+---
 O | X | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 6</summary><pre>
 X | O | O
---+---+---
 4 | O | X
---+---+---
 O | X | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
</details>
<details><summary>Play X at 3</summary><pre>
 1 | O | X
---+---+---
 4 | 5 | O
---+---+---
 O | X | X
</pre>
O responds at 6. Your move:
<details><summary>Play X at 1</summary><pre>
 X | O | X
---+---+---
 4 | O | O
---+---+---
 O | X | X
</pre>
O responds at 5. Your move:
<details><summary>Play X at 4</summary><pre>
 X | O | X
---+---+---
 X | O | O
---+---+---
 O | X | X
</pre><b>Draw. Best possible result against a perfect opponent.</b>
</details>
</details>
<details><summary>Play X at 4</summary><pre>
 O | O | X
---+---+---
 X | 5 | O
---+---+---
 O | X | X
</pre>
O responds at 1. Your move:
<details><summary>Play X at 5</summary><pre>
 O | O | X
---+---+---
 X | X | O
---+---+---
 O | X | X
</pre><b>Draw. Best possible result against a perfect opponent.</b>
</details>
</details>
<details><summary>Play X at 5</summary><pre>
 O | O | X
---+---+---
 4 | X | O
---+---+---
 O | X | X
</pre>
O responds at 1. Your move:
<details><summary>Play X at 4</summary><pre>
 O | O | X
---+---+---
 X | X | O
---+---+---
 O | X | X
</pre><b>Draw. Best possible result against a perfect opponent.</b>
</details>
</details>
</details>
<details><summary>Play X at 4</summary><pre>
 1 | O | O
---+---+---
 X | 5 | 6
---+---+---
 O | X | X
</pre>
O responds at 3. Your move:
<details><summary>Play X at 1</summary><pre>
 X | O | O
---+---+---
 X | O | 6
---+---+---
 O | X | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 5</summary><pre>
 O | O | O
---+---+---
 X | X | 6
---+---+---
 O | X | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 6</summary><pre>
 O | O | O
---+---+---
 X | 5 | X
---+---+---
 O | X | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
</details>
<details><summary>Play X at 5</summary><pre>
 O | O | 3
---+---+---
 4 | X | 6
---+---+---
 O | X | X
</pre>
O responds at 1. Your move:
<details><summary>Play X at 3</summary><pre>
 O | O | X
---+---+---
 O | X | 6
---+---+---
 O | X | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 4</summary><pre>
 O | O | O
---+---+---
 X | X | 6
---+---+---
 O | X | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 6</summary><pre>
 O | O | O
---+---+---
 4 | X | X
---+---+---
 O | X | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
</details>
<details><summary>Play X at 6</summary><pre>
 1 | O | O
---+---+---
 4 | 5 | X
---+---+---
 O | X | X
</pre>
O responds at 3. Your move:
<details><summary>Play X at 1</summary><pre>
 X | O | O
---+---+---
 4 | O | X
---+---+---
 O | X | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 4</summary><pre>
 O | O | O
---+---+---
 X | 5 | X
---+---+---
 O | X | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 5</summary><pre>
 O | O | O
---+---+---
 4 | X | X
---+---+---
 O | X | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
</details>
</details>
</details>
<details><summary>Play X at 9</summary><pre>
 1 | 2 | 3
---+---+---
 4 | O | 6
---+---+---
 7 | 8 | X
</pre>
O responds at 5. Your move:
<details><summary>Play X at 1</summary><pre>
 X | O | 3
---+---+---
 4 | O | 6
---+---+---
 7 | 8 | X
</pre>
O responds at 2. Your move:
<details><summary>Play X at 3</summary><pre>
 X | O | X
---+---+---
 4 | O | O
---+---+---
 7 | 8 | X
</pre>
O responds at 6. Your move:
<details><summary>Play X at 4</summary><pre>
 X | O | X
---+---+---
 X | O | O
---+---+---
 7 | O | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 7</summary><pre>
 X | O | X
---+---+---
 O | O | O
---+---+---
 X | 8 | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 8</summary><pre>
 X | O | X
---+---+---
 O | O | O
---+---+---
 7 | X | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
</details>
<details><summary>Play X at 4</summary><pre>
 X | O | 3
---+---+---
 X | O | 6
---+---+---
 O | 8 | X
</pre>
O responds at 7. Your move:
<details><summary>Play X at 3</summary><pre>
 X | O | X
---+---+---
 X | O | 6
---+---+---
 O | O | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 6</summary><pre>
 X | O | O
---+---+---
 X | O | X
---+---+---
 O | 8 | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 8</summary><pre>
 X | O | O
---+---+---
 X | O | 6
---+---+---
 O | X | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
</details>
<details><summary>Play X at 6</summary><pre>
 X | O | O
---+---+---
 4 | O | X
---+---+---
 7 | 8 | X
</pre>
O responds at 3. Your move:
<details><summary>Play X at 4</summary><pre>
 X | O | O
---+---+---
 X | O | X
---+---+---
 O | 8 | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 7</summary><pre>
 X | O | O
---+---+---
 4 | O | X
---+---+---
 X | O | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 8</summary><pre>
 X | O | O
---+---+---
 4 | O | X
---+---+---
 O | X | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
</details>
<details><summary>Play X at 7</summary><pre>
 X | O | 3
---+---+---
 4 | O | 6
---+---+---
 X | O | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 8</summary><pre>
 X | O | 3
---+---+---
 4 | O | 6
---+---+---
 O | X | X
</pre>
O responds at 7. Your move:
<details><summary>Play X at 3</summary><pre>
 X | O | X
---+---+---
 4 | O | O
---+---+---
 O | X | X
</pre>
O responds at 6. Your move:
<details><summary>Play X at 4</summary><pre>
 X | O | X
---+---+---
 X | O | O
---+---+---
 O | X | X
</pre><b>Draw. Best possible result against a perfect opponent.</b>
</details>
</details>
<details><summary>Play X at 4</summary><pre>
 X | O | O
---+---+---
 X | O | 6
---+---+---
 O | X | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 6</summary><pre>
 X | O | O
---+---+---
 4 | O | X
---+---+---
 O | X | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
</details>
</details>
<details><summary>Play X at 2</summary><pre>
 O | X | 3
---+---+---
 4 | O | 6
---+---+---
 7 | 8 | X
</pre>
O responds at 1. Your move:
<details><summary>Play X at 3</summary><pre>
 O | X | X
---+---+---
 4 | O | O
---+---+---
 7 | 8 | X
</pre>
O responds at 6. Your move:
<details><summary>Play X at 4</summary><pre>
 O | X | X
---+---+---
 X | O | O
---+---+---
 O | 8 | X
</pre>
O responds at 7. Your move:
<details><summary>Play X at 8</summary><pre>
 O | X | X
---+---+---
 X | O | O
---+---+---
 O | X | X
</pre><b>Draw. Best possible result against a perfect opponent.</b>
</details>
</details>
<details><summary>Play X at 7</summary><pre>
 O | X | X
---+---+---
 O | O | O
---+---+---
 X | 8 | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 8</summary><pre>
 O | X | X
---+---+---
 O | O | O
---+---+---
 7 | X | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
</details>
<details><summary>Play X at 4</summary><pre>
 O | X | O
---+---+---
 X | O | 6
---+---+---
 7 | 8 | X
</pre>
O responds at 3. Your move:
<details><summary>Play X at 6</summary><pre>
 O | X | O
---+---+---
 X | O | X
---+---+---
 O | 8 | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 7</summary><pre>
 O | X | O
---+---+---
 X | O | 6
---+---+---
 X | O | X
</pre>
O responds at 8. Your move:
<details><summary>Play X at 6</summary><pre>
 O | X | O
---+---+---
 X | O | X
---+---+---
 X | O | X
</pre><b>Draw. Best possible result against a perfect opponent.</b>
</details>
</details>
<details><summary>Play X at 8</summary><pre>
 O | X | O
---+---+---
 X | O | 6
---+---+---
 O | X | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
</details>
<details><summary>Play X at 6</summary><pre>
 O | X | O
---+---+---
 4 | O | X
---+---+---
 7 | 8 | X
</pre>
O responds at 3. Your move:
<details><summary>Play X at 4</summary><pre>
 O | X | O
---+---+---
 X | O | X
---+---+---
 O | 8 | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 7</summary><pre>
 O | X | O
---+---+---
 4 | O | X
---+---+---
 X | O | X
</pre>
O responds at 8. Your move:
<details><summary>Play X at 4</summary><pre>
 O | X | O
---+---+---
 X | O | X
---+---+---
 X | O | X
</pre><b>Draw. Best possible result against a perfect opponent.</b>
</details>
</details>
<details><summary>Play X at 8</summary><pre>
 O | X | O
---+---+---
 4 | O | X
---+---+---
 O | X | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
</details>
<details><summary>Play X at 7</summary><pre>
 O | X | 3
---+---+---
 4 | O | 6
---+---+---
 X | O | X
</pre>
O responds at 8. Your move:
<details><summary>Play X at 3</summary><pre>
 O | X | X
---+---+---
 4 | O | O
---+---+---
 X | O | X
</pre>
O responds at 6. Your move:
<details><summary>Play X at 4</summary><pre>
 O | X | X
---+---+---
 X | O | O
---+---+---
 X | O | X
</pre><b>Draw. Best possible result against a perfect opponent.</b>
</details>
</details>
<details><summary>Play X at 4</summary><pre>
 O | X | O
---+---+---
 X | O | 6
---+---+---
 X | O | X
</pre>
O responds at 3. Your move:
<details><summary>Play X at 6</summary><pre>
 O | X | O
---+---+---
 X | O | X
---+---+---
 X | O | X
</pre><b>Draw. Best possible result against a perfect opponent.</b>
</details>
</details>
<details><summary>Play X at 6</summary><pre>
 O | X | O
---+---+---
 4 | O | X
---+---+---
 X | O | X
</pre>
O responds at 3. Your move:
<details><summary>Play X at 4</summary><pre>
 O | X | O
---+---+---
 X | O | X
---+---+---
 X | O | X
</pre><b>Draw. Best possible result against a perfect opponent.</b>
</details>
</details>
</details>
<details><summary>Play X at 8</summary><pre>
 O | X | 3
---+---+---
 4 | O | 6
---+---+---
 O | X | X
</pre>
O responds at 7. Your move:
<details><summary>Play X at 3</summary><pre>
 O | X | X
---+---+---
 O | O | 6
---+---+---
 O | X | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 4</summary><pre>
 O | X | O
---+---+---
 X | O | 6
---+---+---
 O | X | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 6</summary><pre>
 O | X | O
---+---+---
 4 | O | X
---+---+---
 O | X | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
</details>
</details>
<details><summary>Play X at 3</summary><pre>
 1 | 2 | X
---+---+---
 4 | O | O
---+---+---
 7 | 8 | X
</pre>
O responds at 6. Your move:
<details><summary>Play X at 1</summary><pre>
 X | O | X
---+---+---
 4 | O | O
---+---+---
 7 | 8 | X
</pre>
O responds at 2. Your move:
<details><summary>Play X at 4</summary><pre>
 X | O | X
---+---+---
 X | O | O
---+---+---
 7 | O | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 7</summary><pre>
 X | O | X
---+---+---
 O | O | O
---+---+---
 X | 8 | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 8</summary><pre>
 X | O | X
---+---+---
 O | O | O
---+---+---
 7 | X | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
</details>
<details><summary>Play X at 2</summary><pre>
 1 | X | X
---+---+---
 O | O | O
---+---+---
 7 | 8 | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 4</summary><pre>
 O | 2 | X
---+---+---
 X | O | O
---+---+---
 7 | 8 | X
</pre>
O responds at 1. Your move:
<details><summary>Play X at 2</summary><pre>
 O | X | X
---+---+---
 X | O | O
---+---+---
 O | 8 | X
</pre>
O responds at 7. Your move:
<details><summary>Play X at 8</summary><pre>
 O | X | X
---+---+---
 X | O | O
---+---+---
 O | X | X
</pre><b>Draw. Best possible result against a perfect opponent.</b>
</details>
</details>
<details><summary>Play X at 7</summary><pre>
 O | 2 | X
---+---+---
 X | O | O
---+---+---
 X | O | X
</pre>
O responds at 8. Your move:
<details><summary>Play X at 2</summary><pre>
 O | X | X
---+---+---
 X | O | O
---+---+---
 X | O | X
</pre><b>Draw. Best possible result against a perfect opponent.</b>
</details>
</details>
<details><summary>Play X at 8</summary><pre>
 O | 2 | X
---+---+---
 X | O | O
---+---+---
 O | X | X
</pre>
O responds at 7. Your move:
<details><summary>Play X at 2</summary><pre>
 O | X | X
---+---+---
 X | O | O
---+---+---
 O | X | X
</pre><b>Draw. Best possible result against a perfect opponent.</b>
</details>
</details>
</details>
<details><summary>Play X at 7</summary><pre>
 1 | 2 | X
---+---+---
 O | O | O
---+---+---
 X | 8 | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 8</summary><pre>
 1 | 2 | X
---+---+---
 O | O | O
---+---+---
 7 | X | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
</details>
<details><summary>Play X at 4</summary><pre>
 O | 2 | 3
---+---+---
 X | O | 6
---+---+---
 7 | 8 | X
</pre>
O responds at 1. Your move:
<details><summary>Play X at 2</summary><pre>
 O | X | O
---+---+---
 X | O | 6
---+---+---
 7 | 8 | X
</pre>
O responds at 3. Your move:
<details><summary>Play X at 6</summary><pre>
 O | X | O
---+---+---
 X | O | X
---+---+---
 O | 8 | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 7</summary><pre>
 O | X | O
---+---+---
 X | O | 6
---+---+---
 X | O | X
</pre>
O responds at 8. Your move:
<details><summary>Play X at 6</summary><pre>
 O | X | O
---+---+---
 X | O | X
---+---+---
 X | O | X
</pre><b>Draw. Best possible result against a perfect opponent.</b>
</details>
</details>
<details><summary>Play X at 8</summary><pre>
 O | X | O
---+---+---
 X | O | 6
---+---+---
 O | X | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
</details>
<details><summary>Play X at 3</summary><pre>
 O | 2 | X
---+---+---
 X | O | O
---+---+---
 7 | 8 | X
</pre>
O responds at 6. Your move:
<details><summary>Play X at 2</summary><pre>
 O | X | X
---+---+---
 X | O | O
---+---+---
 O | 8 | X
</pre>
O responds at 7. Your move:
<details><summary>Play X at 8</summary><pre>
 O | X | X
---+---+---
 X | O | O
---+---+---
 O | X | X
</pre><b>Draw. Best possible result against a perfect opponent.</b>
</details>
</details>
<details><summary>Play X at 7</summary><pre>
 O | 2 | X
---+---+---
 X | O | O
---+---+---
 X | O | X
</pre>
O responds at 8. Your move:
<details><summary>Play X at 2</summary><pre>
 O | X | X
---+---+---
 X | O | O
---+---+---
 X | O | X
</pre><b>Draw. Best possible result against a perfect opponent.</b>
</details>
</details>
<details><summary>Play X at 8</summary><pre>
 O | 2 | X
---+---+---
 X | O | O
---+---+---
 O | X | X
</pre>
O responds at 7. Your move:
<details><summary>Play X at 2</summary><pre>
 O | X | X
---+---+---
 X | O | O
---+---+---
 O | X | X
</pre><b>Draw. Best possible result against a perfect opponent.</b>
</details>
</details>
</details>
<details><summary>Play X at 6</summary><pre>
 O | 2 | O
---+---+---
 X | O | X
---+---+---
 7 | 8 | X
</pre>
O responds at 3. Your move:
<details><summary>Play X at 2</summary><pre>
 O | X | O
---+---+---
 X | O | X
---+---+---
 O | 8 | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 7</summary><pre>
 O | O | O
---+---+---
 X | O | X
---+---+---
 X | 8 | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 8</summary><pre>
 O | O | O
---+---+---
 X | O | X
---+---+---
 7 | X | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
</details>
<details><summary>Play X at 7</summary><pre>
 O | 2 | 3
---+---+---
 X | O | 6
---+---+---
 X | O | X
</pre>
O responds at 8. Your move:
<details><summary>Play X at 2</summary><pre>
 O | X | O
---+---+---
 X | O | 6
---+---+---
 X | O | X
</pre>
O responds at 3. Your move:
<details><summary>Play X at 6</summary><pre>
 O | X | O
---+---+---
 X | O | X
---+---+---
 X | O | X
</pre><b>Draw. Best possible result against a perfect opponent.</b>
</details>
</details>
<details><summary>Play X at 3</summary><pre>
 O | O | X
---+---+---
 X | O | 6
---+---+---
 X | O | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 6</summary><pre>
 O | O | 3
---+---+---
 X | O | X
---+---+---
 X | O | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
</details>
<details><summary>Play X at 8</summary><pre>
 O | 2 | 3
---+---+---
 X | O | 6
---+---+---
 O | X | X
</pre>
O responds at 7. Your move:
<details><summary>Play X at 2</summary><pre>
 O | X | O
---+---+---
 X | O | 6
---+---+---
 O | X | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 3</summary><pre>
 O | 2 | X
---+---+---
 X | O | O
---+---+---
 O | X | X
</pre>
O responds at 6. Your move:
<details><summary>Play X at 2</summary><pre>
 O | X | X
---+---+---
 X | O | O
---+---+---
 O | X | X
</pre><b>Draw. Best possible result against a perfect opponent.</b>
</details>
</details>
<details><summary>Play X at 6</summary><pre>
 O | 2 | O
---+---+---
 X | O | X
---+---+---
 O | X | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
</details>
</details>
<details><summary>Play X at 6</summary><pre>
 1 | 2 | O
---+---+---
 4 | O | X
---+---+---
 7 | 8 | X
</pre>
O responds at 3. Your move:
<details><summary>Play X at 1</summary><pre>
 X | O | O
---+---+---
 4 | O | X
---+---+---
 7 | 8 | X
</pre>
O responds at 2. Your move:
<details><summary>Play X at 4</summary><pre>
 X | O | O
---+---+---
 X | O | X
---+---+---
 O | 8 | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 7</summary><pre>
 X | O | O
---+---+---
 4 | O | X
---+---+---
 X | O | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 8</summary><pre>
 X | O | O
---+---+---
 4 | O | X
---+---+---
 O | X | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
</details>
<details><summary>Play X at 2</summary><pre>
 1 | X | O
---+---+---
 4 | O | X
---+---+---
 O | 8 | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 4</summary><pre>
 O | 2 | O
---+---+---
 X | O | X
---+---+---
 7 | 8 | X
</pre>
O responds at 1. Your move:
<details><summary>Play X at 2</summary><pre>
 O | X | O
---+---+---
 X | O | X
---+---+---
 O | 8 | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 7</summary><pre>
 O | O | O
---+---+---
 X | O | X
---+---+---
 X | 8 | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 8</summary><pre>
 O | O | O
---+---+---
 X | O | X
---+---+---
 7 | X | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
</details>
<details><summary>Play X at 7</summary><pre>
 1 | 2 | O
---+---+---
 4 | O | X
---+---+---
 X | O | X
</pre>
O responds at 8. Your move:
<details><summary>Play X at 1</summary><pre>
 X | O | O
---+---+---
 4 | O | X
---+---+---
 X | O | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 2</summary><pre>
 O | X | O
---+---+---
 4 | O | X
---+---+---
 X | O | X
</pre>
O responds at 1. Your move:
<details><summary>Play X at 4</summary><pre>
 O | X | O
---+---+---
 X | O | X
---+---+---
 X | O | X
</pre><b>Draw. Best possible result against a perfect opponent.</b>
</details>
</details>
<details><summary>Play X at 4</summary><pre>
 1 | O | O
---+---+---
 X | O | X
---+---+---
 X | O | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
</details>
<details><summary>Play X at 8</summary><pre>
 1 | 2 | O
---+---+---
 4 | O | X
---+---+---
 O | X | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
</details>
<details><summary>Play X at 7</summary><pre>
 1 | 2 | 3
---+---+---
 4 | O | 6
---+---+---
 X | O | X
</pre>
O responds at 8. Your move:
<details><summary>Play X at 1</summary><pre>
 X | O | 3
---+---+---
 4 | O | 6
---+---+---
 X | O | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 2</summary><pre>
 O | X | 3
---+---+---
 4 | O | 6
---+---+---
 X | O | X
</pre>
O responds at 1. Your move:
<details><summary>Play X at 3</summary><pre>
 O | X | X
---+---+---
 4 | O | O
---+---+---
 X | O | X
</pre>
O responds at 6. Your move:
<details><summary>Play X at 4</summary><pre>
 O | X | X
---+---+---
 X | O | O
---+---+---
 X | O | X
</pre><b>Draw. Best possible result against a perfect opponent.</b>
</details>
</details>
<details><summary>Play X at 4</summary><pre>
 O | X | O
---+---+---
 X | O | 6
---+---+---
 X | O | X
</pre>
O responds at 3. Your move:
<details><summary>Play X at 6</summary><pre>
 O | X | O
---+---+---
 X | O | X
---+---+---
 X | O | X
</pre><b>Draw. Best possible result against a perfect opponent.</b>
</details>
</details>
<details><summary>Play X at 6</summary><pre>
 O | X | O
---+---+---
 4 | O | X
---+---+---
 X | O | X
</pre>
O responds at 3. Your move:
<details><summary>Play X at 4</summary><pre>
 O | X | O
---+---+---
 X | O | X
---+---+---
 X | O | X
</pre><b>Draw. Best possible result against a perfect opponent.</b>
</details>
</details>
</details>
<details><summary>Play X at 3</summary><pre>
 1 | O | X
---+---+---
 4 | O | 6
---+---+---
 X | O | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 4</summary><pre>
 1 | O | 3
---+---+---
 X | O | 6
---+---+---
 X | O | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 6</summary><pre>
 1 | O | 3
---+---+---
 4 | O | X
---+---+---
 X | O | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
</details>
<details><summary>Play X at 8</summary><pre>
 1 | 2 | 3
---+---+---
 4 | O | 6
---+---+---
 O | X | X
</pre>
O responds at 7. Your move:
<details><summary>Play X at 1</summary><pre>
 X | 2 | O
---+---+---
 4 | O | 6
---+---+---
 O | X | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 2</summary><pre>
 O | X | 3
---+---+---
 4 | O | 6
---+---+---
 O | X | X
</pre>
O responds at 1. Your move:
<details><summary>Play X at 3</summary><pre>
 O | X | X
---+---+---
 O | O | 6
---+---+---
 O | X | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 4</summary><pre>
 O | X | O
---+---+---
 X | O | 6
---+---+---
 O | X | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 6</summary><pre>
 O | X | O
---+---+---
 4 | O | X
---+---+---
 O | X | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
</details>
<details><summary>Play X at 3</summary><pre>
 1 | 2 | X
---+---+---
 4 | O | O
---+---+---
 O | X | X
</pre>
O responds at 6. Your move:
<details><summary>Play X at 1</summary><pre>
 X | 2 | X
---+---+---
 O | O | O
---+---+---
 O | X | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 2</summary><pre>
 1 | X | X
---+---+---
 O | O | O
---+---+---
 O | X | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 4</summary><pre>
 O | 2 | X
---+---+---
 X | O | O
---+---+---
 O | X | X
</pre>
O responds at 1. Your move:
<details><summary>Play X at 2</summary><pre>
 O | X | X
---+---+---
 X | O | O
---+---+---
 O | X | X
</pre><b>Draw. Best possible result against a perfect opponent.</b>
</details>
</details>
</details>
<details><summary>Play X at 4</summary><pre>
 1 | 2 | O
---+---+---
 X | O | 6
---+---+---
 O | X | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
<details><summary>Play X at 6</summary><pre>
 1 | 2 | O
---+---+---
 4 | O | X
---+---+---
 O | X | X
</pre>
<b>O wins. Collapse a section above and try a different branch.</b>
</details>
</details>
</details>

