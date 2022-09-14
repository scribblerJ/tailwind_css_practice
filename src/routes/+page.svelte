<script>
    let picture = "https://images.unsplash.com/photo-1570295999919-56ceb5ecca61?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=880&q=80";
    // let picture = "../../profile_img.png";
    function createTextLevel1(text){
        return '<div class="pb-4 text-yellow-500 font-bold text-xl">'+text+'</div>';
    }
    function createTextLevel2(text){
        return '<div class="font-bold text-l">'+text+'</div>';
    }
    function createTextLevel3(text){
        return '<div class="pr-4 font-bold text-xs">'+text+'</div>';
    }
    function createTextLevel4(text){
        return '<div class="text-gray-400 text-xs">'+text+'</div>';
    }
    function createTextLevel5(text){
        return '<li class="text-gray-400 text-xs">'+text+'</li>';
    }
    function createStars(num_of_filled_stars){
        return '<span class="fa fa-star text-xs"></span>'.repeat(num_of_filled_stars) + '<span class="fa fa-star text-xs" style="color:grey;"></span>'.repeat(5-num_of_filled_stars);
    }

</script>
<main>
    <div class="p-12">
        <div class="grid grid-cols-3">
            <div>
                <div class="py-12" >
                    <img class="w-24 shadow-1xl rounded-full object-scale-down" src={picture} alt="프로필 이미지">
                </div>
                <div class="py-8">
                    {@html createTextLevel1("Info")}

                    <div class="py-2">
                        {@html createTextLevel3("Address")}
                        {@html createTextLevel4("20 kimlin Court,")}
                        {@html createTextLevel4("Poughkeppsl 12603 United States")}
                    </div>                    
                    <div class="py-2">
                        {@html createTextLevel3("Phone")}
                        {@html createTextLevel4("(845) 763-1264")}
                    </div>                    
                    <div class="py-2">
                        {@html createTextLevel3("Email")}
                        {@html createTextLevel4("elsa_william2@gamil.com")}
                    </div>
                </div>
                <div class="py-12">
                    {@html createTextLevel1("Skills")}
                    <div class="py-2">
                        {@html createTextLevel3("Patient Education")}
                        {@html createStars(4)}
                    </div>
                    <div class="py-2">
                        {@html createTextLevel3("Physical Evaluations")}
                        {@html createStars(3)}
                    </div>
                    <div class="py-2">
                        {@html createTextLevel3("Treatment Plans")}
                        {@html createStars(2)}
                    </div>
                    <div class="py-2">
                        {@html createTextLevel3("Excellent Communications")}
                        {@html createStars(5)}
                    </div>
                    

                </div>
            </div>
            <div class="col-span-2">
                <div class="py-14">
                    <div class="font-bold text-4xl">Elsa Williams</div>
                    <div class="text-gray-400">Physical Therapist</div>
                </div>
                <div class="py-12">
                    {@html createTextLevel1("Profile")}
                    <div >
                        {@html createTextLevel4("Lorem ipsum dolor sit amet consectetur adipisicing elit. Esse unde facere sint illum itaque sapiente neque qui obcaecati commodi tempore. Voluptatem rerum ipsam exercitationem, distinctio amet officiis aspernatur cumque facilis.Lorem ipsum dolor sit amet consectetur adipisicing elit. Esse unde facere sint illum itaque sapiente neque qui obcaecati commodi tempore. Voluptatem rerum ipsam exercitationem, distinctio amet officiis aspernatur cumque facilis.")}
                    </div>
                </div>                
                <div class="py-8">
                    {@html createTextLevel1("Employment History")}
                    {@html createTextLevel2("Physical Therapist, care Mount Medical Center")}
                    <div class="flex">
                        {@html createTextLevel3("Jan 2013 - Aug 2019")}
                        {@html createTextLevel4("I. Poughkeepsie")}
                    </div>
                    <ul class="list-disc pl-10 pb-10">
                        {@html createTextLevel5("She has a primary degree in law")}
                        {@html createTextLevel5("She has a primary degree in law")}
                        {@html createTextLevel5("She has a primary degree in law")}
                        {@html createTextLevel5("She has a primary degree in law")}
                    </ul>
                    {@html createTextLevel2("Physical Therapist, care Mount Medical Center")}
                    <div class="flex">
                        {@html createTextLevel3("Jan 2013 - Aug 2019")}
                        {@html createTextLevel4("I. Poughkeepsie")}
                    </div>
                    <ul class="list-disc pl-10">
                        {@html createTextLevel5("She has a primary degree in law")}
                        {@html createTextLevel5("She has a primary degree in law")}
                        {@html createTextLevel5("She has a primary degree in law")}
                        {@html createTextLevel5("She has a primary degree in law")}
                    </ul>
                </div>
                <div class="py-8"> 
                    {@html createTextLevel1("Education")}
                    {@html createTextLevel2("Marist Colege Master of Physical Therapy")}
                    <div class="flex">
                        {@html createTextLevel3("Jan 2013 - Aug 2019")}
                        {@html createTextLevel4("I. Poughkeepsie")}
                    </div>
                    <ul class="list-disc pl-10 pb-10">
                        {@html createTextLevel5("She has a primary degree in law")}
                        {@html createTextLevel5("She has a primary degree in law")}
                        {@html createTextLevel5("She has a primary degree in law")}
                        {@html createTextLevel5("She has a primary degree in law")}
                    </ul>
                </div>
            </div>
        </div>
    </div>
</main>

<style>
    .ulist{
        list-style: square;
    }
</style>