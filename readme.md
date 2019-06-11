# Atomic Grid
### A lightweight grid system using CSS grid.

Atomic grid is a familiar responsive grid system inspired by [Tachyons](tachyons.io) and designed using modern CSS.
Atomic grid takes the complexity out of the CSS grid system and gives you the old school grid system you know and love.
No fluff was added, so the whole thing weighs in at less than 10K minified.

---

## Preview

https://codepen.io/leetheguy/pen/LKYpqb

---

## The Grid

The grid system consists of a grid wrapper, offset and span tags.
Rows are implied and not needed.
The grid wrapper comes in 3 flavors including 12-column, 20-column, and 24-column.

    <div class="g-12"></div>
    <div class="g-20"></div>
    <div class="g-24"></div>

---

## Automatic

Atomic Grid will automatically fill in cells from left to right.
Rows are implied and not needed.
When the end of the row is reached a new one will be started.

    <div class="g-12">
      <div>col</div>
      <div>col</div>
      <div>col</div>
    </div>

---

## Offsets

The grid cells can be offset from 1 to 23 columns with `go[1-23]`.

    <div class="g-12">
      <div class="go4">column</div>
    </div>

Multiple cells can be offset from the row beginning.

    <div class="gs12 g-12">
      <div class="go2">column 3</div>
      <div class="go5">column 6</div>
      <div class="go8">column 9</div>
      <div class="go11">column 12</div>
    </div>

---

## Spans

The grid cells can span multiple columns with `gs[1-24]`.

    <div class="g-12">
      <div class="gs4">rule</div>
      <div class="gs4">of </div>
      <div class="gs4">thirds</div>
    </div>

---

## Nesting

Grids can be easily nested.

    <div class="g-12">
      <div class="g-12 gs4 go4">
        <div class="gs4">column</div>
        <div class="gs4">column</div>
        <div class="gs4">column</div>
      </div>
    </div>

---

## Responsive

Atomic Grid uses the same media queries as tachyons `-ns` for not small, `-m` for medium, and `-l` for large.

    <div class="g-12">
      <div class="gs6 gs3-m gs2-l">column</div>
      <div class="gs6 gs3-m gs2-l">column</div>
      <div class="gs6 gs3-m gs2-l">column</div>
      <div class="gs6 gs3-m gs2-l">column</div>
      <div class="gs6 gs3-m gs2-l">column</div>
      <div class="gs6 gs3-m gs2-l">column</div>
      <div class="gs6 gs3-m gs2-l">column</div>
      <div class="gs6 gs3-m gs2-l">column</div>
      <div class="gs6 gs3-m gs2-l">column</div>
      <div class="gs6 gs3-m gs2-l">column</div>
      <div class="gs6 gs3-m gs2-l">column</div>
      <div class="gs6 gs3-m gs2-l">column</div>
    </div>
