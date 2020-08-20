### CSS Transformations, Transitions, and Animations

###### Transforms

The transform property comes in two different settings, two-dimensional and three-dimensional. Each of these come with their own individual properties and values.

`div {
  -webkit-transform: scale(1.5);
     -moz-transform: scale(1.5);
       -o-transform: scale(1.5);
          transform: scale(1.5);
}`

2D Transforms
* 2D Rotate
* 2D Scale
* 2D Translate
* 2D Skew

###### Transition Duration

The duration in which a transition takes place is set using the transition-duration property. The value of this property can be set using general timing values, including seconds (s) and milliseconds (ms). These timing values may also come in fractional measurements, .2s for example.\

`.box {
  background: #2db34a;
  border-radius: 6px;
  transition-property: background, border-radius;
  transition-duration: .2s, 1s;
  transition-timing-function: linear;
}`

###### 8 Simple CSS3 Transitions

1. Fade in
2. Change Color
3. Grow & Shrink
4. Rotate Elements
5. Square to Circle
6. 3D shadow
7. Swing
8. Inset Border










