# JavaScript A* PathFinder Algorithm

## Sync Usage

```html

<script src="AStar.js"></script>
<script>
    const path2 = await PathFinder.AStar.search([
        [1, 1, 1, 1, 1],
        [1, 1, 1, 1, 1],
        [1, 1, 1, 1, 1],
        [1, 1, 1, 1, 1],
        [1, 1, 1, 1, 1]
    ], {x: 1, y: 1}, {x: 3, y: 3}, {
        closest: false,
        heuristic: AStar.heuristics.manhattan,
        diagonal: false,
        sync: true
    });
    console.log(path2);
</script>
```

## Async Usage

```html

<script src="AStar.js"></script>
<script>
    const path2 = await PathFinder.AStar.search([
        [1, 1, 1, 1, 1],
        [1, 1, 1, 1, 1],
        [1, 1, 1, 1, 1],
        [1, 1, 1, 1, 1],
        [1, 1, 1, 1, 1]
    ], {x: 1, y: 1}, {x: 3, y: 3}, {
        closest: false,
        heuristic: AStar.heuristics.manhattan,
        diagonal: false,
        sync: false
    });
    console.log(path2);
</script>
```