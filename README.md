# Customer Review Extension
 Customer Review Extension
Platform: Opencart 3.x
Extension File Name Format : opencart_3x_customer_review_v{IN-PROGRESS-VERSION-NUMBER}.ocmod.zip
Versions:
	0.0.0 - Project Repo created
	0.0.1 - install.xml added
		0.0.1.1 - Install the extension in extension installer.
		0.0.1.2 - Enable the extension in extension modification.
		0.0.1.3 - Goto user group & permissions. Enable the new extension
		0.0.1.4 - Left link should be visible.
	0.0.2 - Admin
		0.0.2.1 - Language file
			0.0.2.1.1 - admin/language/en-gb/extension/module/customer_review.php
		0.0.2.2 - List page
			0.0.2.2.1 - admin/model/extension/module/customer_review.php :: getTotalCustomerReviews() & getCustomerReviews()
			0.0.2.2.2 - admin/controller/extension/module/customer_review.php :: index() & getList()
				- sort + page
				- breadcrumb
				- add & delete link
				- filter_data array
				- getTotalRecords()
				- getRecords() with filter_data
				- iteration of result data into view data... [array]
				- common alert messages --> warning + success
				- incase of bulk selection, pass the selected list also
				- pagination + results + header + footer + columns
			0.0.2.2.2 - admin/view/template/extension/module/customer_reviews_list.twig
			0.0.2.2.3 - Test the list page flow. Left link on click, show right side list page with add & edit clickable

