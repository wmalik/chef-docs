.. This is an included how-to. 

The following example shows how to use the |resource package| resource to install an application named "app" and ensure that the correct packages are installed for the correct platform:

.. code-block:: ruby

   package "app_name" do
     action :install
   end
   
   case node[:platform]
   when "ubuntu","debian"
     package "app_name-doc" do
       action :install
     end
   when "centos"
     package "app_name-html" do
       action :install
     end
   end
