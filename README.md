# LSB Steganography

This Project Describes the use of LSB Steganography.<br>
Do check the python script written to implement lsb steganography<br>
<p style="color: grey" >#./stego -f &lt;filename.png&gt; -e &lt;secret_message&gt; -p &lt;Password (Optional) &gt; : To embed a secret message. <br>
#./stego -f &lt; secretfile.png &gt; -x -p &lt; Password supplied &gt; : To extract the secret message.<br>
#Note : Even if you passed a blank field in the -p argument,while creating a secret file, you must append a -p while extracting the message. </P>

STEGANOGRAPHY  comes  from  the  Greek  Words:  STEGANOS  –  “Covered”,  GRAPHIE  –  “Writing”.
The sender hides his/her message within an image/audio/video.Since the algorithm uses the lease significant bit to hide the secret message the change is undectable by a naked eye.<br>
The various types of steganography include:
<br>
<ul>
  <li>Image Steganography</li>
  <li>Audio  Steganography</li>
  <li>Video Steganography</li>
  <li>Text files Steganography</li>
  </ul>
<br>
Types of Images:
<ul>
  <li>Black and white</li>
  <li>Geryscale</li>
  <li>RGB</li>
</ul>
<p>In a gray scale image each pixel is represented in 8 bits. The last bit in a pixel is called as Least Significant bit as its value will affect the pixel value only by “1”. So, this property is used to hide the data in the image. If anyone have considered last two bits as LSB bits as they will affect the pixel value only by “3”</P>
<p>  The  LSB  embedding  approach  has become the basis of many techniques that hide messages within multimedia carrier data. LSB embedding may even be  applied  in  particular  data  domains  –  for  example,  embedding  a  hidden  message  into  the  color  values  of  RGB bitmap data</p>

<h3>Let's study the application of LSB on a Greyscale Image</h3>
<p>In a Greyscale image, each pixel is represented by 8 bits, while in a RGB it is 24 bits</p>
<p>Suppose the following are some of the bits in a Grayscale image</p>
<p>11110011 <br> 11011011 <br>10110110 <br> 11011100<br>11011111 <br> 11010111 <br> 00100110 <br> 01000011</p>
<h4>You wish to hide "A" in it. The ascii value of "A" is 10000001.</h4>
<p>The algorithm simply replaces the last bit of the bytes with the consecutive bits of the letter "A", Giving us </p>
<p>11110011 <br> 11011010 <br>10110110 <br> 11011100<br>11011110 <br> 11010110 <br> 00100110 <br> 01000011</p>

<h2>Steganalysis</h2>
<p>Steganalysis is the study of detecting messages hidden using steganography</p>
<p>LSB Steganography can be detected by looking at the histograms of the files</p>
<p>Also lossy compression technique can render LSB Steganography useless to an extent, so lossless compression techniques should be used</p>


