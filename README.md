# 4june
june repository
using System;
using System.Collections.Generic;
using System.Linq;
using System.Web;
using System.Data.Entity;

namespace workingwith_Migrations.Models
{
    public class Mycontext:DbContext
    {
        public Mycontext() : base("MyContextDB") { }
        public virtual DbSet<Course> Courses { get; set; }
        public virtual DbSet<Enrollment> Enrollments { get; set; }
        public virtual DbSet<Student> Students { get; set; }
    }
}
