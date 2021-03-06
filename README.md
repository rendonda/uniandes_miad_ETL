# uniandes_miad_ETL
Clase modelado de datos y ETL

# Notes on submitting jupyter notebooks as markdown wiki pages in Github

1. Save Jupyter notebook as .ipynb file
1. In the conda terminal (already inside your virtual environment), enter `jupyter nbconvert <your-jupyter-notebook.ipynb> --to markdown --output-dir=<your-output-dir>`
  This will create a folder named `<your-output-dir>` that contains a file `<your-jupyter-notebook.md>` with the contents of your Jupyter notebook as markdown file as well as a folder containing all the images in your notebook.

1. In your Github repo, on the main page, click on "Add file" and select "Upload files". This is because the markdown document will not include any images generated by code, and these have to be manually added. Skip this step if there are no images
1. Drag and drop the folder that contains your images onto the upload files page and wait until they are uploaded. Commit/Save changes.
1. In the Github wiki, create a new page and give it an appropriate title.
1. Open the markdown file `<your-jupyter-notebook.md>` in your editor in your local machine, and copy-and-paste its content to the content of the wiki page that you created above.
1. To add images, you have to do the following changes: 
   * Any image that was embedded in the markdown will look like `![png](<path/to/your/.png>)`.
   * Change it to `[[https://github.com/MIAD-Modelo-Datos/<your-id>/raw/main/<path/to/your/.png>]]`