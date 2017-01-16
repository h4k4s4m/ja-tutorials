---
layout: post
title:  "Gitlab SSH"
categories: Advanced Bluebeam
published: true
---
{:.post-intro}
**Tutorial on adding SSH Key to GitLab to easily clone and pull changes.**

### Add your SSH Key

1. Go to your git lab profile settings and click on SSH Keys  
{% include image.html image="gitlab/gitlab-ssh-page.gif" class="img-xlarge" %}  
2. Open up a terminal window and paste the following command to copy your SSH Key to your clipboard:  `pbcopy < ~/.ssh/id_rsa.pub` 
    - NOTE: If you have not created an SSH key yet, follow my Git-SSH tutorial first to generate an SSH Key
3. Go back to your browser and paste your SSH key under `Key`. 
4. Add a Title and click on `Add Key`
{% include image.html image="gitlab/paste-ssh-key.gif" class="img-xlarge" %}

### Clone using SSH
1. Navigate to the project
2. Copy the SSH Link
{% include image.html image="gitlab/copy-repo-ssh.gif" class="img-xlarge" %}
3. Open up a terminal and cd into the directory where you will clone this repository.
4. Run `git clone {ssh path}`
    - ex: `git clone git@uclax.bootcampcontent.com:UCLA-Coding-Boot-Camp/01-17-Class-Content.git` 
    
That's about it. You will no longer be require to input your username and password when cloning and pulling from gitlab. 