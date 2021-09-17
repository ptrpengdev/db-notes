# db-notes

Relational Algebra in DBMS: Operations Symbol. **Source** (https://www.guru99.com/relational-algebra-dbms.html#15)
```
SELECT(σ)
Projection(π)
Rename (ρ)
Union operation (υ)
Set Difference (-)
Intersection (∩)
Cartesian product(X)
Inner Join:
Theta Join: ⋈θ.  r ⋈θ s = σθ (r x s) do a cross product and then select specific row within cross product
EQUI join:
NATURAL JOIN (⋈)
OUTER JOIN 
Left Outer Join(A  B)
Right Outer Join: ( A  B )
Full Outer Join: ( A  B)

![Image of Eq Relational Algebra] 
(https://github.com/ptrpengdev/db-notes/blob/main/Screen%20Shot%202021-09-17%20at%203.00.25%20PM.png)
```


### Projection

remove column that aren't needed for further calculation.

### sharding
```
  Against large database, part of relation can split up into shard. Original = Shard1 υ Shard2 υ Shard3
```

### Theta Join: ⋈θ
```
r(name, spent) and s(name, available)
To determine people who not in debt, we might write
r ⋈θ s where θ = (r.name = s.name and r.spent < s.available)
```
