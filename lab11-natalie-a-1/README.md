# Lab 11: Sierpinski Triangles

In this lab, you will generate images of Sierpinski Triangles using JavaFX and recursion. Then, you'll add these images to a web page, host this web page to a server on a Google Cloud Platform virtual machine, and then setup your server so that your page can be accessed using a static IP address.

## 1-Setting up the VM
You'll need to create a new VM on GCP and start-up an nginx webserver. Refer back to Lab 10 instructions if needed.

### Reserve a Static IP address and Attach it to the VM
To make sure that your VM IP address does not change when the instance is stopped, you'll need to reserve a static IP address for your VM instance. 
For instructions on how to accomplish this, refer to [GCP documentation](https://cloud.google.com/compute/docs/ip-addresses/reserve-static-external-ip-address)

## 2-Drawing Sierpinski Triangles

More information about these triangles can be found at [Wikipedia](https://en.wikipedia.org/wiki/Sierpi%C5%84ski_triangle). Use JavaFX to generate Sierpinski Triangles of a specific depth. Then, export the graphics as an image using JavaFX. Generate at least 9 images for different depths from 0 to 8. You can find a lot of online resources on generating these triangles using recursion in JavaFX.

## 3-Building Webpages

In this repository, you'll find a directory called `html`. Inside this directory, you'll find another directory called `images`. First, copy the images you generated from the previous step to this directory. Then, modify the file `index.html` so that it displays these images.

## 4-Hosting Webpages 

After having your web page files in `html` directory, you need to make them visible to `nginx` so that you can access the webpage from the browser. The easiest way of doing this is to copy these files to the default directory where nginx looks for web pages. You can do this as follows:

```
sudo cp -a ~/lab11-username/html/. /var/www/html/
```

## 5-Submission 

For this lab, submit the link to your web page to canvas (similar to last lab). 

