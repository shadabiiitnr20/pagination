## Simple Pagination using ReactJS


# Steps to be followed

- Use Bootstrap CDN Link to style the webapp. (https://react-bootstrap.netlify.app/docs/getting-started/introduction/)
- First declare the state variables - posts, loading, currentPage, postsPerPage.
- Fetch the posts and set the posts state variable using the response. Use useEffect to fetch the posts.
- Create a new component Posts and pass posts and loading as props and display the list of posts in Posts component. for styling use -> list-group, list-group-item.
- Define the following in the root file where state varibale are defined.
    - const indexOfLastPost = currentPage * postsPerPage;
    - const indexOfFirstPost = indexOfLastPost - postsPerPage;
    - const currentPosts = posts.slice(indexOfFirstPost, indexOfLastPost);
- pass the currentPosts array as props to the Posts component.

- Create a new component for Pagination. refer the logic in the file. Use Paginate function to change the pageNumber.