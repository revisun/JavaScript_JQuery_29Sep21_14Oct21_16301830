HTML 5
----------------------------------------------------------------------------

    Hyper Text MarkUp Language

        is documentation language.
        generating html documents that can be shared across the http protocol and
        are rendered on a browser.

        Hyper Text
            Formated and Plain Text
            Graphiscs
            Links

        The content is wrapped inside an html element represented by an open and close tag

            <tag>content</tag>

    Lab Setup

        VSCode
        Chrome

    HTML document

        <!DOCTYPE html>

        <html>
            <head>
                <!-- meta data -->
            </head>
            <body>
                <!-- actual content -->
            </body>
        </html>

    HTML basics
        heading,paragraphs and typology
    
        h1 h2 h3 h4 h5 h6           block elements
        p                           block elements
        b i u strong em             inline elements
        sup sub                     inline elements
        blockquote                  block element
        div                         block element
        span                        inline eleemnt

    HTML Lists

        ol          Ordered list
            type    attribute takes 1,a,A,I,i as values
        ul          Unordered list
            type    attribute takes dot,circle,square as values   

        li          list item is a sub-tag of ol and ul.

    HTML Tables    
        table                   to create a table
                border          attribute takes 1 to 5
                width           attribute takes a value in px/%/em/pt/in/cm
                heigth          attribute takes a value in px/%/em/pt/in/cm
                cellspacing     attribute takes a valeu in px/%/em/pt/in/cm and controls the spacing between two 
                                cells
                cellpadding     attribute takes a valeu in px/%/em/pt/in/cm and controls the spacing between the 
                                cell border and its content

        caption                 sub-element to give a heading to the table
        tr                      table row is a sub element representing one row
        th                      table hader cell, a sub-element of tr
        td                      table data cell, a sub-element of tr
                rowspan         attribute of th and td representing the number of rows to be occupied default is 1
                colspan         attribute of th and td representing the number of columns to be occupied default is 1
       
    HTML Media

        img         inline element that injects an image into the page
             src    attribute of img tag to hold the relative or absolute or virtual path 
                    of the image

        audio       inline element to inject an audio
        video       inline element to inject a video
        source      sub-element of audio and video to supply the audio file or video file
                    a single audio or video element can house anynumber of source tags
                    each represeting a different format of audio or video.
            src     attibute of source to hold the relative or absolute or virtual path 
                    of the audio or video file

        iframe      used to embed an external web page into our own web page.
            src     attribute to hold the web address of the webpage you wish to embed.

    HTML Links
        a           amchor tag 
            href    attribute takes the target file path.
            target  attribute takes _self/_blank/iframeName

    HTML Form Elements
        form                is used to group a set of fields that have to be submitted to a server program.
            action          attribute takes the path of the server program to which the data has to be submitted
            method          attribute that takes GET/POST
        
        label               used to carry a text related to a field like field names
            for             attribute takes th id of the input element to which the label is related to.

        input               used to create a form field control that enable inputting data
            type            text
                            file
                            password
                            checkbox
                            radio

                            number
                            range
                            decimal
                            email
                            date
                            datetime-locale
            
            id              attribute is used to give an id to the input element.
            name            attribute is sued to give a field name that is carried along with its value to the server.
            value           attribute takes the initial vbalue of the field

            required        attribute ensures that the field is given a value mandatly
            min             attribute that takes a minimum possible value for type="number/decimal/date"
            max             attribute that takes a maximum possible value for type="number/decimal/date"
            minlength       attribute that takes a minimum length of the value while type="text"
            maxlength       attribute that takes a maximum length of the value while type="text"
            pattern         attribute that takes a reglar expression to validate the value while type="text"

        textarea            used to accpet multi line text
        
        select              used to create a drop-down or a list box
            multiple        attribute makes the drop-down into a list enabling multiple option selection
         option             is a sub-element of select used to provide the options
            value           attribute of option tag that takes the value to be submitted if this option is selected

        button              used to create a push button
            type            submit      (defualt)
                            reset
                            button

    HTML Layouts and sematic elements

        <header>    - Defines a header for a document or a section
        <nav>       - Defines a set of navigation links
        <section>   - Defines a section in a document
        <article>   - Defines an independent, self-contained content
        <aside>     - Defines content aside from the content (like a sidebar)
        <footer>    - Defines a footer for a document or a section
        <details>   - Defines additional details that the user can open and close on demand
        <summary>   - Defines a heading for the <details> element
        <figure>    - Defines a self-contained content, like illustrations, diagrams, photos, code listings..etc
        <figcaption>- Defines a caption for a <figure> element.
        <time>	    - Defines a date/time


    HTML entities

        Result	        Description	            Entity Name	    Entity Number
        =============================================================================
        non-breaking    space	                &nbsp;	        &#160;
        <	            less than	            &lt;	        &#60;
        >	            greater than	        &gt;	        &#62;
        &	            ampersand	            &amp;	        &#38;
        "	            double quotation mark	&quot;      	&#34;
        '	            single quotation mark 	&apos;      	&#39;
        ¢	            cent	                &cent;	        &#162;
        £	            pound	                &pound;	        &#163;
        ¥	            yen	                    &yen;	        &#165;
        €	            euro	                &euro;	        &#8364;
        ©	            copyright	            &copy;	        &#169;
        ®	            registered trademark	&reg;	        &#174;
    
CSS 3 
-------------------------------------------------------------------------------------
    CSS 3 - Intro
    -----------------------------------

        Cascading Style Sheet

        purpose is to provide styling to an html document.

        + CSS offers common uniform properties unlike html
        + CSS can provide styling across grouped elements.
        + CSS can isolate styling from content. It adds to maintainability.
        
        Inline Style Sheet

            it is applied using 'style' attribute.

            <tagName style="css-property:value;css-property:value;">
                content
            </tagName>

        Embeded Style Sheet

            it is applied using a tag called <style></style>, style elements
            is a sub-element of <head></head>

            <head>
                <style>
                    selector {
                        css-property:value;
                        css-property:value;
                    }
                </style>
            </head>

            selector is a string that qualfies the elements to be applied with the style.

            1. Tag Name
                    each tag name itself is a selector.
                    
                    tagName{
                        css-property:value;
                    }

            2. Attribute
                    attribute selector groups elements having the mentioned attribute.
                    
                    [attributeName]{
                        css-property:value;
                    }
                    
                    [attributeName=""]{
                        css-property:value;
                    }

            3. Class

                    is any usr defiend string. that should start with dot(.)
                    to apply the class on a element the element class attribute 
                    should be assigned with the class name.

                    .className{
                        css-property:value;
                    }

                    <tagName class="className">
                    </tagName>
            4. Id
                    if a style swhould be applied to an elemnt hving 
                    a specific id, then id selector is sued.

                    #id{
                        css-property:value;
                    }

            5. Psuedo


        External Style Sheet

            style is defiend in a seperate file with extension .css
            and that cna be linked to any number of html pages using
                
                <link href="fileName.css" rel="stylesheet" />


    CSS - unit of measure
    ------------------------------------

        absolute		(irrespective of screen size)
            in
            mm
            cm
            pt		1 in = 72 pt
            pc		1 in = 6  pc   1 pc = 12 pt
        
        relative 	(to screen size)
        
            px
            
            %
            
            em			relative the font-size
                        1 em = complete font-size
                                            
                        font-size: 12pt;
                        width: 8em;	8*12pt = 96pt;
                        
            vh			1% of viewport height
            vw			1% of viewport width
            vmin		min of vh or vw


    CSS Box Model Properties
    -----------------------------------
        margin
        margin-top
        margin-bottom
        margin-left
        margin-right

        border              border-size border-style border-color
        border-top
        border-bottom
        border-left
        border-right

        padding             space between the contetn and the elemnt border
        padding-top
        padding-bottom
        padding-left
        padding-right

        border-radius       radius of the corners of the element
        border-top-left-radius
        border-top-right-radius
        border-bottom-left-radius
        border-bottom-right-radius

        width
        height
        min-width
        min-height
        max-width
        max-height

        display             inline/block/inline-block

        position            relative / absolute

        top
        left
        bottom
        right
        z-index

    CSS background color and image related properties
    ----------------------------------------------
        background-color
        color
        background-image
        background-repeat       no-repeat/repeat/repeat-x/repeat-y
        background-position
        background-attachment    fixed/scroll
              
    CSS font related properties
    -----------------------------------
        font-family
        font-size
        font-variant		normal or small-caps
        font-weight			bold or bolder or boldest 
                            or any number like 300,400,500..etc
        font-style			italic or oblique
        
    CSS Text related Proeprties
    -----------------------------------
        color
        direction
        letter-spacing
        word-spacing
        text-align
        text-indent
        text-decoration		none | underline | line-through | overline
        
    table related css prperties
    ------------------------------------
        border-collapse			collapse or seperate
        border-spacing
        caption-side			top left right bottom
        
    CSS list related properties
    ----------------------------------

        list-style-type			disc	circle	square	none	for ul
                                decimal							for ol
                                decimal-leading-zero	
                                lower-alpha
                                upper-alpha
                                lower-roman
                                upper-roman
        list-style-position		outside or inside
        list-style-image:		url('imgs/note.png')
        marker-offset
        
  
    controlling scroll bars
    ------------------------------------
        
        overflow
                    visible
                    scroll
                    auto
                    hidden
                    
    CSS Operators
    -------------------------------------
        s1		applies to elements that have s1 as tag name
        .s1		applies to elements that have s1 as class
        #s1		applies to elements that have s1 as id

        s1,s2	applies to elements that match both selectors
        s1 s2	applies to all elements that match s2 and are inside s1
        s1>s2	applies to all elements that match s2 whose parent is s1
        s1+s2	applies to all elements that match s2 and are immediately after s1
        s1~s2	applies to every element that match s2 and is preceded by s1

                        applies to all elements that have
                        ------------------------------------
        [s1]			 s1 as attribute
        [s1='v1']		 s1 attrib with v1 value
        [s1~='v1']		 s1 attrib value containes word v1
        [s1*='v1']		 s1 attrib value containes word v1
        [s1!='v1']		 s1 attrib value not equal to v1
        [s1^='v1']		 s1 attrib value starts with the word v1
        [s1$='v1']		 s1 attrib value ends with the word v1

        Psuedo selectors
        ----------------------------------------------------------------------------
        input:enabled	Selects every enabled <input> element
        p:first-child	Selects every <p> element that is the first child 
                        of its parent
        p::first-letter	Selects the first letter of every <p> element
        p::first-line	Selects the first line of every <p> element
        p:first-of-type	Selects every <p> element that is the first <p> 
                        element of its parent
        input:focus		Selects the input element which has focus
        a:hover			Selects links on mouse over
        input:in-range	Selects input elements with a value within a specified range

        input:indeterminate		
                        Selects input elements that are in an indeterminate state

        input:invalid	Selects all input elements with an invalid value
        input:optional	Selects input elements with no "required" attribute

        p:last-child	Selects every <p> element that is the last child of its parent
        p:last-of-type	Selects every <p> element that is the last <p> element of its parent

        a:link			Selects all unvisited links
        :not(p)			Selects every element that is not a <p> element
        p:nth-child(2)	Selects every <p> element that is the second child of its parent
        p:nth-last-child(2)	
                        Selects every <p> element that is the second child of its parent, 
                        counting from the last child

        p:nth-last-of-type(2)	
                        Selects every <p> element that is the second <p> element of its parent, 
                        counting from the last child
        p:nth-of-type(2)	
                        Selects every <p> element that is the second <p> element of its parent
                        
HTML & CSS Assignment
---------------------------------------------------------------------------

    Digital resume:
        Banner Section
                Photo
                Name
                Contact details
        Skill Set
        Technical Qualifications
        Academic Qualification
        Experience And Recent Projects
        Achivments And Publications
        Personal Details

JavaScript (ES6)
---------------------------------------------------------------------------

    Javascript Basics

            is a scripting language that can execute its scripts
            both on a browser and in a stand alone mode too.

            we need a javascript runtime to execute the script
            without a browser. And NodeJS is one such runtime.

            1. javascript inherits it syntx fgrom c and cpp,hence case sensitive
            2. is a dynamically typed language
                number(integer,floats),string,null,array,undefined,object

        Datatypes
        Variables and scopes (let,var), operators
        Control Structures
        Program Flows
        String, Math, Date
        
    Javascript OOPs
    Javascript Functions
        Arrow Functions
        Memeber Functions and this keyword
        call and apply
        call backs and closures

    Javascript Arrays

    ES6 Enhancements
        Modules
        Template Literals
        Arrow Functions
        Destructuring
        Spread and Rest operators
    
    Javascript Asynchronous Programming
        setInterval
        clearInterval
        setTimeout
        clearTimeout

        async, await and Promise

    Javascript BOM & DOM

        Browser Object Model
            window
                navigator
                    appName
                    appCodeName
                history
                    back()
                    forward()
                location
                    href
                    hostname
                    protocol
                    assign(url)
                document

                alert()
                prompt()
                confirm()
                setInterval()
                clearInterval
                setTimeout()
                clearTimeout()
                open()
                close()

        Document Object Model
            document

                elements
                forms

                createElement()
                removeElement()
                replace(oldEle,newEle)
                append()
                prepand()
                getElementById(id)
                getElementsByName(name)
                querySelector("css-selector")

HTML 5 Jvascript API
---------------------------------------------------------------------------
        GeoLocation
            navigator.geolocation
        Canvas
        Drag and Drop
        Web Stoirage
            localStorage
                .setItem("key","value")
                .getItem("key")
                .removeItem("key")
                .clear()
            sessionStorage
                .setItem("key","value")
                .getItem("key")
                .removeItem("key")
                .clear()

JQuery
---------------------------------------------------------------------------
   
   is a javascript library.

   $("css-selector")        returns a dom element that matches the selector
   $(() => {})              the passed callback is executed once the page is loaded
   $(javascriptObject)      returns the object with additional fucntions of JQuery api

        Event Handling
        ---------------------------

            document.querySelector("#p1").addEventListener('click',()=>{})

            $("#p1").click(()=>{ })
            $("#p1").click()

            $("#p1").toggle(
                ()=>{},()=>{},()=>{},......
            )

            $("#p1").on({
                click:()=>{},
                mouseover:()=>{}......
            })

            $("#p1").off(click)     removes the click event handlet

        Content Access
        -------------------------------

            $("#p1").text()         returns the text content
            $("#p1").text("")       sets the text content

            $("#tb1").val()         returns the value of the text box
            $("#tb1").val(val)      sets the valeu of the text box

            $("#p1").css("border")
            $("#p1").css("border","1px solid black")

            $("#img1").attrib("src")
            $("#img1").attrib("src","imgs/logo1.png")

            $("#img1").prop("src")
            $("#img1").prop("src","imgs/logo1.png")

        Effect Api
        -------------------------------

            show(timeDelay)
            hide(timeDelay)
            toggle(timeDelay)

            fadeIn(timeDelay)
            fadeOut(timeDelay)
            fadeToggle(timeDelay)
            fadeTo(timeDelay,opacity)

            slideUp(timeDelay)
            slideDown(timeDelay)
            slideToggle(timeDelay)

            animate({css-style},timeDelay)

        Dom Manipulation
        -------------------------------
            ${parentElement}.append(element)
            ${parentElement}.prepend(element)

            ${element}.appendTo(parentElement)
            ${element}.prependTo(parentElement)

            ${element1}.after(element2)
            ${element1}.before(element2)

            ${element}.remove()

            ${element}.addClass("css-class")



Bootstrap
---------------------------------------------------------------------------
            
            Bootstrap was developed by Mark Otto and Jacob Thornton at Twitter, 
            and released as an open source product in August 2011 on GitHub.

            Download from : http://getbootstrap.com/

            CDN:

            <link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.7/css/bootstrap.min.css">
            <script src="https://ajax.googleapis.com/ajax/libs/jquery/3.3.1/jquery.min.js"></script>
            <script src="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.7/js/bootstrap.min.js"></script>

            Look Before You Leep
            ----------------------------

                1. html 5 doctype is a must for Bootstrap 3
                2. use lang attributre for html element.
                3. also do set the char set
                4. bootstrap is mobile-first.
                Thus add the view port conf as meta tag.
                
                    <!DOCTYPE html>
                    <html lang="en">
                    <head>
                        <meta charset="utf-8"> 
                        <meta name="viewport" content="width=device-width, initial-scale=1">
                    </head>
                    </html>
                    

            Bootstrap Container classes
            -------------------------------

                .container			creates a fixed width container
                .container-fluid	creates a full fixed width container
                    
                    
            Grid classes
            -------------------------
                
                row		will create a responsive row
                
                col-gridType-gridSize
                    
                    gridType
                        xs (for phones - screens less than 768px wide)
                        sm (for tablets - screens equal to or greater than 768px wide)
                        md (for small laptops - screens equal to or greater than 992px wide)
                        lg (for laptops and desktops - screens equal to or greater than 1200px wide)
                    
                    gridSize	from 1 to 12.
                    
            Bootstrap Typography
            --------------------

                <h1> - <h6>
                <small>
                <mark>
                <abbr>
                <blockquote>
                .blockquote-reverse
                <dl>,<dt>,<dd>
                <code>
                <kbd>
                
                .text-muted
                .text-primary
                .text-success
                .text-info
                .text-warning
                .text-danger
                
                .bg-primary
                .bg-success
                .bg-info
                .bg-warning
                .bg-danger

                .lead			Makes a paragraph stand out	   
                .small			Indicates smaller text (set to 85% of the size of the parent)	   
                .text-left		Indicates left-aligned text	   
                .text-center	Indicates center-aligned text	   
                .text-right		Indicates right-aligned text	   
                .text-justify	Indicates justified text	   
                .text-nowrap	Indicates no wrap text	   
                .text-lowercase	Indicates lowercased text	   
                .text-uppercase	Indicates uppercased text	   
                .text-capitalize	Indicates capitalized text	   
                .list-unstyled	Removes the default list-style and left margin on list items 
                .list-inline	Places all list items on a single line	   
                
            Bootstrap tables  classes
            -------------------------

                .table
                .table-striped
                .table-bordered
                .table-hover
                .table-condensed		saves spaces by reducing cell-padding
                .table-responsive		allows horizontal scrolling on small screens
                
                classes for tr and td for contexual formating
                ---------------------------------------------
                .active		Applies the hover color to the table row or table cell
                .success	Indicates a successful or positive action
                .info		Indicates a neutral informative change or action
                .warning	Indicates a warning that might need attention
                .danger		Indicates a dangerous or potentially negative action
                
            Bootstrap image formating classes
            ----------------------------------------
            .img-rounded	Adds rounded corners to an image 
            .img-circle		Shapes the image to a circle 
            .img-thumbnail	Shapes the image to a thumbnail	
            .img-responsive	Makes an image responsive 

            Bootstrap button formating classes
            ------------------------------------------
                
                .btn
                .btn-default
                .btn-primary
                .btn-success
                .btn-info
                .btn-warning
                .btn-danger
                .btn-link
                    
                .btn-group		groups a set of buttons in a packed contaienr.
                .btn-group-lg
                .btn-group-vertical
                .btn-group-justified
                
            form styling
            ------------------------------
                .form-control	for form elements for auto bootstrap styling
                
                Bootstrap provides three types of form layouts:

                    Vertical form 		(this is default)
                    Inline form			.form-inline
                    Horizontal form		Add class .form-horizontal to the <form> element
                                        Add class .control-label to all <label> elements
                
                Standard rules for all three form layouts:

                    Wrap labels and form controls in <div class="form-group"> (needed for optimum spacing)
                    Add class .form-control to all textual <input>, <textarea>, and <select> elements

                
            Special Contaienrs
            ----------------------------------
            .jumbotron 	 displayed as a grey box with rounded corners. It also enlarges the font sizes of the text inside it.
            
            .well class adds a rounded border around an element with a gray background color and some padding:

                alert alert-success
                alert alert-info
                alert alert-warning
                alert alert-danger
                    
                    will create a closable alert container, add
                    fade and in classes for fade effects.

            card
            tab
            navbar
                    
            Creating a pagination bar
            ------------------------------------

            <ul class="pagination">
                <li><a href="#">1</a></li>
                <li><a href="#">2</a></li>
                <li><a href="#">3</a></li>
                <li><a href="#">4</a></li>
                <li><a href="#">5</a></li>
            </ul>
