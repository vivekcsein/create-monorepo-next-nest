# NestJS & NextJS monorepo project

<h2>
Project initialization
</h2>
<p>
To initialize the project, you need to install Node.js and run these commands in your terminal:
    
    npm i -g pnpm

    pnpm init

</p>

To initialize the project, run:

<p> create "pnpm-workspace.yaml" file at root level

    pnpm-workspace.yaml

    type nul> pnpm-workspace.yaml

</p>
<p>and copy paste following content into it </p>

    packages:
        - 'apps/*'

</p>

<h2>
Create Apps Folder
</h2>

    mkdir apps

<h2> Create NestJS app inside apps folder and use pnpm
</h2>

<p> 
change name of the folder to anything  you like (e.g., server, backend) here i use server
</p>

<p> commands for creating nestjs new project

    cd apps

    nest new server --strict --skip-git --package-manager=pnpm

</p>

<h2> Create NextJS app inside apps folder and use pnpm
</h2>

<p> 
change name of the folder to anything  you like (e.g., client, frontend) here i use client
</p>
<p> commands for creating nextjs new project

    cd ..

    pnpm create next-app@latest client

</p>

<h2> Create tsconfig.json file to configure appropriate between two typescript projects 
</h2>

<p> To add any package to specific project we need to add command in the end --filter=projectname, for example:

    pnpm add @nestjs/config --filter=server

</p>
