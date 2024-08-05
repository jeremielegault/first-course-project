<script>
    import Header from "./UI/Header.svelte";
    import MeetupItem from "./Meetups/MeetupItem.svelte";
    const meetups = [
        {
            id: "m1",
            title: "Coding Bootcamp",
            subtitle: "Learn to code in 2 hours",
            description:
                "In this meetup, we will have some experts teach you coding basics.",
            imageUrl: "https://shorturl.at/uAj2b",
        },
        {
            id: "m2",
            title: "Intro to Web Development",
            subtitle: "Get started with HTML, CSS, and JavaScript",
            description:
                "Join us for an introductory session on web development where you'll learn the fundamentals of building websites with HTML, CSS, and JavaScript.",
            imageUrl: "https://shorturl.at/uAj2b",
        },
        {
            id: "m3",
            title: "Advanced Python Programming",
            subtitle: "Deep dive into Python for data science",
            description:
                "This meetup focuses on advanced Python programming techniques, especially for data science. Perfect for those who already have a basic understanding of Python.",
            imageUrl: "https://shorturl.at/uAj2b",
        },
        {
            id: "m4",
            title: "React.js Workshop",
            subtitle: "Build dynamic web apps with React",
            description:
                "Learn how to create dynamic and interactive web applications using React.js in this hands-on workshop. Suitable for those with some JavaScript experience.",
            imageUrl: "https://shorturl.at/uAj2b",
        },
        {
            id: "m5",
            title: "Machine Learning Basics",
            subtitle: "Introduction to machine learning concepts",
            description:
                "Explore the basics of machine learning in this session. We will cover essential concepts, algorithms, and practical applications of machine learning.",
            imageUrl: "https://shorturl.at/uAj2b",
        },
        {
            id: "m6",
            title: "Full-Stack Development Bootcamp",
            subtitle: "Master both front-end and back-end technologies",
            description:
                "A comprehensive bootcamp covering both front-end and back-end development. Learn how to build complete web applications from scratch using modern technologies.",
            imageUrl: "https://shorturl.at/uAj2b",
        },
    ];
</script>

<Header />
<section id="meetups">
    {#each meetups as meetup}
        <MeetupItem {meetup} />
    {/each}
</section>

<style>
    #meetups {
        margin-top: 5rem;
    }
</style>
