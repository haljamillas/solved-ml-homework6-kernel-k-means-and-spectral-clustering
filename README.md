Download Link: https://assignmentchef.com/product/solved-ml-homework6-kernel-k-means-and-spectral-clustering
<br>
<strong>Kernel K-means and Spectral Clustering</strong>

<ol>

 <li><strong>Homework Objective:</strong> Use whatever your favorite language to code out kernel k-means, spectral clustering (both normalized cut and ratio cut). You should consider spatial similarity and color similarity upon the clustering.</li>

 <li><strong>Data:</strong> Two 100*100 images are provided, and each pixel in the image should be treated as a data point, which means there are 10000 data points in each image.</li>

</ol>

<ul>

 <li><strong>Kernel:</strong> For both kernel k-means and spectral clustering, please use the new kernel defined below to compute the Gram matrix.</li>

</ul>

<em>k </em>(<em>x</em>,<em>x</em>′) = <em>e</em>−γ<em><sub>s</sub></em>∥<em>S</em>(<em>x</em>)−<em>S</em>(<em>x</em>′)∥<sup>2</sup>× <em>e</em>−γ<em><sub>c</sub></em>∥<em>C</em>(<em>x</em>)−<em>C</em>(<em>x</em>′)∥<sup>2</sup>

This new defined kernel is basically multiplying two RBF kernels in order to consider spatial similarity and color similarity at the same time. <em>S </em>(<em>x</em>) is the spatial information (i.e. the coordinate of the pixel) of data <em>x </em>, and <em>C </em>(<em>x</em>) is the color information (i.e. the RGB values) of data <em>x </em>. Both <sup>γ</sup><em><sub>s</sub></em> and γ<em><sub>c</sub></em>  are hyper-parameters which you can tune in your own way.

<h1>IV.            Requirements:​</h1>

<ul>

 <li>Part1: You need to make videos or​ GIF images to show the clustering procedure (visualize the cluster assignments of data points in each iteration, colorize each cluster with different colors) of your kernel k-means and spectral clustering (both normalized cut and ratio cut) programs. (Hint : Numpy can help you to solve the eigenvalue problem.)</li>

 <li>Part2: In addition to cluster data into 2 clusters, try more clusters (e.g. 3 or 4) and show your results. (You also need to make videos ​ or GIF images)​</li>

 <li>Part3: For the initialization of k-means clustering used in kernel k-means, (e.g. k-means++) and spectral clustering (both normalized cut and ratio cut), try different ways and show corresponding results. (You also need to make videos ​ or GIF images)​</li>

 <li>Part4: For spectral clustering (both normalized cut and ratio cut), you can try to examine whether the data points within the same cluster do have the same coordinates in the eigenspace of graph Laplacian or not. You should plot the result and discuss it in the report.</li>

</ul>




<h1>V.            Report:​</h1>

<ul>

 <li>Submit a report in pdf format. The report should be written in English​ .​  Report format:</li>

</ul>

○ a. code with detailed explanations (40%)

■ Paste the screenshot of your functions with comments and explain your code. For example, explain the process to clustering and show different initialization methods, etc.

■ Note that if you don’t explain your code clearly, you cannot get any points in section b and c either.

<ul>

 <li>Part1 (15%) Part2 (5%)</li>

 <li>Part3 (10%)</li>

 <li>Part4 (10%)</li>

</ul>

○ b. experiments settings and results (20%) &amp; discussion (30%)

■ Show everything we asked you to show

<ul>

 <li>Part1 (5%) &amp; (5%)</li>

 <li>Part2 (5%) &amp; (5%)</li>

 <li>Part3 (5%) &amp; (10%)</li>

 <li>Part4 (5%) &amp; (10%)</li>

</ul>

○ c. observations and discussion (10%)

■ Anything you want to discuss, such as comparing the performance between different kernels or the execute time of different settings.

<strong>P.S.</strong> If the zip file name has format error or the report is not in pdf format, a penalty will be imposed (-10). Please submit your homework before the deadline, late​ submission is not allowed.

Note that if you miss any one of the requirements (report, or source code), you cannot get any score!

&#x2666;        Packages allowed in this assignment:

You are only allowed to use numpy, scipy.spatial.distance, package for reading image and visualizing results. Official introductions can be found online.