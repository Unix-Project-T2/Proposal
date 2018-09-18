### Proposal

A one page proposal for our Unix OS semester long project. Latex will be used to create all documents and charts. 

## How to install Latex

I am assuming you all are on an Ubuntu machine. To install the entire texlive suite, copy and paste this command to your terminal.
`sudo apt-get install texlive-full`
Enter your password when prompted and the `y` character when asked. 

## Creating the PDF

Once you have installed the Latex sutie, you now can create the PDF by running the following command:
`pdflatex Proposal.tex`

You'll see the logs as they appear but should terminate successfully. Type the `ls` command. You should now see a few more files than what we began with. Within these files you'll see the output file we want, `Proposal.pdf`. You can open it using `evince Proposal.pdf` or by navigating to the location of the file and double clicking the PDF using Ubuntu's Files GUI.

## Editing, Adding, Commiting, and Pushing

When you are done making your edits to a file, open your terminal and add each specific file you've made edits to by using the following command: `git add FILE1 FILE2 ...` where each file is a file you edited. Then run `git commit FILE1 FILE2 ... -m "your message"`. You need to commit the same files you added from the previous command. Make sure to add a meaning full message between the quotes. An example can be "add more details on motivation". Just make sure it's short and to the point. Finally when you've added and commited your edits, run `git push` to publish your changes. 

## What not to Push

Do not push any .log, .aux, or .pdf files to the repository. Keep them local to your machine. This will avoid merging conflicts that can be a hassle to get through down the road. Only push .tex files please.
