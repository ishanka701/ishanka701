class DataScientist {
    constructor() {
        this.name = "Ishanka Chathuranga Botheju";
        this.role = "Data Science Student";
        this.location = "Sri Lanka 🇱🇰";
        this.education = "BSc (Hons) Data Science";
        this.university = "Your University Name";
        this.interests = [
            "Machine Learning",
            "Data Analytics", 
            "Web Development",
            "AI & Deep Learning"
        ];
        this.currentlyLearning = ["Python", "R", "TensorFlow", "React"];
        this.lookingToCollaborate = true;
    }
    
    getMotivation() {
        return "Turning data into insights, one algorithm at a time! 📊🤖";
    }
    
    sayHi() {
        console.log("Thanks for dropping by! Let's build something amazing together. 🚀");
    }
}

const me = new DataScientist();
me.sayHi();
console.log(me.getMotivation());
