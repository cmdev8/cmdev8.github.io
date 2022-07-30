---
title: "My First Post"
date: 2022-07-30T17:09:09+02:00
draft: false
---

Sample

{{< highlight go "linenos=table,hl_lines=8 15-17,linenostart=199" >}}
// An implementation of Conway's Game of Life.
package main

import (
	"bytes"
	"fmt"
	"math/rand"
	"time"
)

// Field represents a two-dimensional field of cells.
type Field struct {
	s    [][]bool
	w, h int
}

// NewField returns an empty field of the specified width and height.
func NewField(w, h int) *Field {
	s := make([][]bool, h)
	for i := range s {
		s[i] = make([]bool, w)
	}
	return &Field{s: s, w: w, h: h}
}
{{< / highlight >}}

