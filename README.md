# codestar-demo
CodeStar demonstration
1. Log onto the AWS Console
2. Browse to the CodeStar Service
3. Click on **Create New Project**
4. Review the templates available for launch.
5. On the left hand side, check the boxes next to Web Service, and Ruby.
6. Click on the **Ruby (Sinatra)** tile that has **EC2** as the target.
7. Give the project a unique name.
8. Keep **CodeCommit** as the repository, and click **Next**.
9. Review the project details, and click **Create Project**.
10. Select your SSH key pair, and check the box acknowledgement.  Click **Create Project**.
11. Select **AWS Cloud9** for the development environment.  Click **Next**.
12. On the **Set up your AWS Cloud9 environment** page, leave the **t2.micro** checked off, and expand the **Network Settings** option.
13. Select the proper VPC, and subnets to launch your instance in.  Click **Next**.


The environment will take 15 - 20 minutes to set up.

14. Review the dashboard and see what components are available during the project launch.
15. Locate the application endpoint tile.  Click on the endpoint.
16. You will notice the page does not load properly.
17. Browse back to the CodeStar dashboard, and locate the **IDE** icon on the left.  Click on it.
18. Open the Cloud9 IDE.
19. Expand your project in Cloud9.  Locate the server.rb file.
20. Add **set :bind '0.0.0.0'** to the file after the **require** statments.
21. Save the file.
22. In Cloud9, go to the terminal, and run **git add server.rb**, **git commit -m "some message"**, and **git push origin master**.
23. Browse back to the CodeStar console.  Notice **Continuous Deployment** tile.  You should see changes happening from your commit.
24. Once all the steps have been run, locate the endpoint, and you should see an output message, **Hello World!**
25. 