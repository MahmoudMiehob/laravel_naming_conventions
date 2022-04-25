# laravel_naming_conventions
--------------
* Naming Controller :
    
    * Controllers should be in singular case, no spacing between words, and end with "Controller"
        
        * For example: AuthController, UserController
        * Bad examples: UsersController 
    
* database tables :
    
    * DB tables should be in lower case, with underscores to separate words
        
        * For example: posts, project_tasks,
        * Bad examples: all_posts, Posts 

* Pivot tables :
    
    * Pivot tables should be all lower case
        
        * For example: post_user, task_user
        * Bad examples: users_posts 

* Table columns names :
    
    * Table column names should be in lower case, and snake_case 
        
        * For example: post_body, id
        * Bad examples: blog_post_created_at, forum_thread_title 

* Primary Key :
    
    * This should normally be id

* Foreign Keys :
    
    * Foreign keys should be the model name (singular), with '_id'
        
        * For example: comment_id, user_id.

* Variables :
    
    * Normal variables should typically be in camelCase
        
        * For example: $users , $bannedUsers 
        * Bad examples: $all_banned_users
 
* Naming Models :
    
    * A model should be in singular, no spacing between words, and capitalised.
        
        * For example: User
        * Bad examples: users

* Model Methods :
    
    * Methods should be camelCase but the first character lower case.
        
        * For example: public function get(), public function getAll() 
        * Bad examples: public function GetPosts(), public function get_posts()

* Relationships : 
    
    * hasOne or belongsTo relationship (one to many)
        
        * These should be singular form and follow the same naming conventions of normal model methods 
            * For example: public function postAuthor(), public function phone().
    
    * hasMany, belongsToMany, hasManyThrough (one to many) 
        * These should be the same as the one to many naming conventions, however, it should be in plural.
            * For example: public function comments(), public function roles() 

* Method naming :
    * CRUD
        * Get     =>  index()  =>  /photos
        * Get     =>  create() =>  /photos/create
        * Post    =>  store()  =>  /photos
        * Get     =>  show()   =>  /photos/{photo}
        * Get     =>  edit()   =>  /photos/{photo}/edit
        * Put     =>  update() =>  /photos/{photo}
        * Delete  =>  destroy()=>  /photos/{photo}

* Traits :
    * Traits should be be adjective words.
        * For example: Notifiable

* Blade view files :
    * Blade files should be in lower case, snake_case
        * For example: all.blade.php    



