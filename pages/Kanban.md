- #.v-eisenhower-matrix
	- [[IU]]
	  collapsed:: true
		- #+BEGIN_QUERY
		  {:query [:find (pull ?b [*])
		    :where
		      [?tag :block/name ?tag-name]
		      [(= ?tag-name "IU")]
		      [?page :block/name ?page-name]
		      [(= ?page-name "2024.02.19")]
		      [?page-block :block/page ?page]
		      [?page-block :block/refs ?b]
		      [?b :block/refs ?tag]
		    ]
		  }
		  #+END_QUERY
	- [[IX]]
	- [[UX]]
	- [[XX]]