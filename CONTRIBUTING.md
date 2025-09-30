<!-- markdownlint-disable MD024 -->
# Contribution Guidelines

Thanks for your interest in contributing to our project. This page will give you a quick overview of how things are organized and, most importantly, how to get involved. Everyone is welcome to contribute, and we value everybody's contribution.

## Table of contents

1. [Add a project](#add-a-project)
2. [Update a project](#update-a-project)
3. [Improve metadata collection](#improve-metadata-collection)
4. [Improve markdown generation](#improve-markdown-generation)
5. [Create your own best-of list](#improve-markdown-generation)
6. [Code of conduct](#code-of-conduct)

## Add a project

If you like to suggest or add an example, choose one of the following ways:

- Suggest an example by opening an issue: Please use the suggest project template from the [issue page](https://github.com/WAVI-ice-sheet-model/example-registry/issues/new/choose) and fill in the requested information.
- Add an example by modifying the [projects.yaml](https://github.com/WAVI-ice-sheet-model/example-registry/blob/main/projects.yaml) and submitting a pull request with your addition. This can also be done directly via the [Github UI](https://github.com/WAVI-ice-sheet-model/example-registry/edit/main/projects.yaml).

Before opening an issue or pull request, please ensure that you adhere to the following guidelines:

- Please make sure that the project was not already added or suggested to this list. You can ensure this by searching the projects.yaml, the Readme, and the issue list.
- Add the project to the `projects.yaml` and never to the `README.md` file directly. Use the yaml format and the properties documented in the [project properties](#project-properties) section below to add a new project, for example:
    ```yaml
    - name: PIG-CES
      github_id: WAVI-ice-sheet-model/example-name
      labels: ["Idealised", "Antarctic"]
      category: EKI
    ```
- Please create an individual issue or pull request for each example.
- Please use the following title format for the issue or pull request: `Add project: project-name`.
- If a project doesn't fit into any of the pre-existing categories, it should go under the `Others` category by not assigning any category. You can also suggest a new category via the add or update category template on the [issue page](https://github.com/WAVI-ice-sheet-model/example-registry/issues/new/choose).

## Update a project

If you like to suggest or contribute a project update, choose one of the following ways:

- Suggest a project update by opening an issue: Please use the update project template from the [issue page](https://github.com/WAVI-ice-sheet-model/example-registry/issues/new/choose) and fill in the requested information.
- Update a project by modifying the [projects.yaml](https://github.com/WAVI-ice-sheet-model/example-registry/blob/main/projects.yaml) and submitting a pull request with your changes. This can also be done directly via the [Github UI](https://github.com/WAVI-ice-sheet-model/example-registry/edit/main/projects.yaml).

Before opening an issue or pull request, please ensure that you adhere to the following guidelines:

- Only update the project in the `projects.yaml` and never to the `README.md` file directly. Use the yaml format and the properties documented in the [project properties](#project-properties) section below to update a new project.
- Please create an individual issue or pull request for each project.
- Please use the following title format for the issue or pull request: `Update project: project-name`.

## Project properties

<table>
    <tr>
        <th>Property</th>
        <th>Description</th>
    </tr>
    <tr>
        <td><code>name</code></td>
        <td>Name of the project. This name is required to be unique on the best-of list.</td>
    </tr>
    <tr>
        <td><code>github_id</code></td>
        <td>Github ID of the project based on user or organization and the repository name, e.g. <code>best-of-lists/best-of-generator</code>.</td>
    </tr>
    <tr>
        <td colspan="2"><b>Optional Properties:</b></td>
    </tr>
    <tr>
        <td><code>category</code></td>
        <td>Category that this project is most related to. You can find all available category IDs in the <code>projects.yaml</code> file. The project will be sorted into the <code>Others</code> category if no category is provided.</td>
    </tr>
    <tr>
        <td><code>labels</code></td>
        <td>List of labels that this project is related to. You can find all available label IDs in the <code>projects.yaml</code> file.</td>
    </tr>
    <tr>
</table>


## Code of Conduct

All members of the project community must abide by the [Contributor Covenant, version 2.0](./.github/CODE_OF_CONDUCT.md). Only by respecting each other we can develop a productive, collaborative community. Instances of abusive, harassing, or otherwise unacceptable behavior may be reported by contacting a project maintainer.
