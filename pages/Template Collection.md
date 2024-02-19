- Daily Template
  template:: Daily
  template-including-parent:: false
	- [[Kanban]]
	- [[3 vital things I decide to do]] #.ol
	- [[3 good things I have done]] #.ol
- ```yaml
  title: Important & Urgent
  - pages
      - *
  - tasks
  	- TODO
      - or DOING
  - blocktags
    - IU
  ```
	- #+BEGIN_QUERY
	  ;; WARNING: yaml has no leading hypen eg '- pages'
	  
	  ;; **ERROR: tasks not valid with pages command use blocks command instead
	  
	  
	  ;; **ERROR: blocktags not valid with pages command use blocks command instead
	  
	  {
	  :title [:b "Important & Urgent"]
	  :query [:find (pull ?block [*])
	  :where
	  [?block :block/name ?pagename]
	  ]
	  }
	  #+END_QUERY