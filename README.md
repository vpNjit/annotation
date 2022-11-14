<h1>ANNOTATION</h1>
<h2>Kitchen</h2>
<p>To get the images needed for annotation we <b>web scraped</b> product pictures from <b>amazon</b></p>
<img src="https://github.com/vpNjit/annotation/blob/main/img/kitchen.png">

<h2>Setting up DEXTR</h2>
<p>In order to use the <b>DEXTR tool</b>, you will need to install <b>Anaconda</b> from their website: 
<br><i>https://www.anaconda.com/products/distribution</i></p>
<p>After completing the <b>installation</b>, <b>restart</b> your computer for the necessary files to load to memory.
Go to the <b>start menu</b> and search for the <b>Anaconda prompt</b>. Launch it and enter the following command to clone the <b>dextr</b> tool from github arrays of data:
<br><i>git clone https://github.com/karan-shr/DEXTR-AnnoTool</i>
<br>Navigate into the DEXTR folder:
<br><i>cd DEXTR-AnnoTool</i>
<br>Set up the conda environment:
<br><i>conda env create -n dextr_annotool -f conda_env.yml</i>
<br>Navigate into the models folder:
<br><i>cd models/</i>
<br>Download the dextr model:
<br><i>chmod +x download_dextr_model.sh
./download_dextr_model.sh
</i>
<br>At this point you may encounter errors related to missing <b>tensorflow module</b>. To resolve this you need to <b>uninstall</b> and <b>install</b> tensorflow again. Use this command to install:
<br><i>Pip3 install tensorflow</i>
<br>To demonstrate using the <b>annotation</b> user interface use the command:
<br><i>python annotate.py -c anno_cfg.yml</i>
<br>For a computer with multiple <b>GPU’s</b> you can specify which one to use using the command:
<br><i>CUDA_VISIBLE_DEVICES=0 python annotate.py -c anno_cfg.yml</i></p><br>

<b>Loading the images for annotation</b><br>
	<img src="https://github.com/vpNjit/annotation/blob/main/img/ann1.png"><br>
<b>Creating labels</b><br>
	<img src="https://github.com/vpNjit/annotation/blob/main/img/ann2.png"><br>
<b>Annotating</b><br>
	<img src="https://github.com/vpNjit/annotation/blob/main/img/ann3.png"><br>
	<img src="https://github.com/vpNjit/annotation/blob/main/img/ann4.png"><br>
