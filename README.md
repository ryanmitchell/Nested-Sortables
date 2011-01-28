Nested Sortables
===========

Nested Sortables is a class to provide sortable-like function on a nested element.

![Screenshot](http://url_to_project_screenshot)

How to use
----------

Include the script at the top of your page, and then set up an instance with a reference to a UL or other similar nested element:

	new NestedSortables('nestedElement', {
		collapse: true,
		events: {
			onStart: function(el){
				console.log('started sorting');
			},
			onComplete: function(el){
				console.log('stopped sorting');
			}
		}
	});
	

Options
-------

This class accepts the following options:

*childTag* (string)
The type of tag to recognise as a child element (e.g. 'li')

*ghost* (boolean)
Whether to add a ghost element while sorting

*childStep* (integer)
Attempts to become a parent/child if this amount is moved left/right

*handleClass* (null or string)
The classname of the element to use for dragging

*collapse* (boolean)
Whether to provide collapsing of sub-elements

*collapseClass* (string)
The classname to add to a collapsed element

*expandKey* (string)
The keypress required with click to make an element expand/collapse

*lock* (options are: null, parent, depth, class)
Whether to lock sorting to a parent, to the same depth, to a certain class or to within the list

*lockClass* (string)
The classname to use if the lock option is set to class


Credits
-------

This code is effectively a MooTools 1.3 port of some 1.1 code written by CrazyDave. I can't provide a link to his website 
as it doesn't seem to exist any more. But on the off-chance he reads this - thanks for some great code!
