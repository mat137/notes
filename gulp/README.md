```JavaScript
var gulp = require('gulp');
var sass = require('gulp-ruby-sass');
var sourcemaps = require('gulp-sourcemaps');

gulp.task('sass', function(){
// console.log("hejS");
  return sass('scss/**/*.scss', {style: 'expanded', sourcemap:true})
  .on('error', sass.logError)
  .pipe(sourcemaps.init())
  .pipe(sourcemaps.write())
  .pipe(gulp.dest('css'));

});

gulp.task('watch', function(){
  gulp.watch('scss/**/*.scss', ['sass']);
})


//wtyczka ktora robi za nas pranie :)
var gulp = require('gulp');
gulp.task('pranie', function() {
console.log('robię pranie');
});

var gulp = require('gulp');
var sass = require('gulp-sass');
//wtyczka do parsowania scss na css
gulp.task('sass', function() {
  return gulp.src('scss/style.scss')
  .pipe(sass())
  .pipe(gulp.dest('css'))
});
//wtyczka do parsowania automatycznego na css
gulp.task('watch', function(){
  gulp.watch('scss/**/*.scss', ['sass']);
});
//wtyczka szukajaca bledy w js
//wymagana instalacja jshint oraz gulp-jshint
const jshint = require('gulp-jshint');

gulp.task('lint', function(){
  return gulp.src('./lib/*.js')
  .pipe(jshint())
  .pipe(jshint.reporter('default'));
});



```
