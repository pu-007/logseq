- #.v-eisenhower-matrix
	- [[IU]]
	  collapsed:: true
		- ```yaml
		  title: Important & Urgent
		  - blocks
		  	- *
		  - blocktags
		  	- IU
		  ```
			- #+BEGIN_QUERY
			  ;; WARNING: yaml has no leading hypen eg '- pages'
			  {
			  :title [:b "Important & Urgent"]
			  :query [:find (pull ?block [*])
			  :where
			  [?block :block/content ?blockcontent]
			  [?block :block/page ?page]
			  [?page :block/name ?pagename]
			  ]
			  }
			  #+END_QUERY
	- [[IX]]
	- [[UX]]
	- [[XX]]