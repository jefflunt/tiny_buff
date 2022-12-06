see `lib/tiny_buff.rb`

- add a cursor (not visual, but a char index)
- inserts/deletes should move marks, possibly removing them in a delete
- inserts/deletes should move selections, possibly removing some/all of them in a delete
- add yanks (creating of dynamic char ranges as selections)
- add highlights (reusable visually highlighted ranges, which maybe is just a
  selection that some other tool will highlight visually?)
- consider whether or not everything should be a range
  - marks can be single or multi-character marks
  - selections are already ranges
  - yanks are a special kind of range that is created when copying something
  - highlights are just selections displayed visually, which is some other
    tool's job
